cmake_minimum_required(VERSION 3.5)
set ( ARDUINO_HTTP_CLIENT_SRC
      "src/b64.cpp"
      "src/HttpClient.cpp"
      "src/URLEncoder.cpp"
      "src/WebSocketClient.cpp"
)

idf_component_register(SRCS ${ARDUINO_HTTP_CLIENT_SRC}
                    INCLUDE_DIRS "src/."
                    REQUIRES "arduino" # Library requires Arduino
                    )

project(ArduinoHttpClient)
