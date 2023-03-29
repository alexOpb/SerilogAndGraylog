# Serilog & Graylog Integration

To run:
1. Open terminal in solution folder.
2. Run `docker-compose up -d` to start Graylog.
3. Configure Graylog:
   - Access UI: http://localhost:9000 (login: admin, password: qwertyuiop)
   - Add Inputs: System > Inputs > GELF UDP > name it, set port to 12201
   - Click "Show received messages"
4. Run app, open Swagger UI, and use GET method.
5. Logs appear in: log file (Logs folder), console, and Graylog.
