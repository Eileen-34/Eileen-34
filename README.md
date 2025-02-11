# Eileen_Aylin API

This is a personal API that provides an overview of Eileen_Aylin's skills, interests, and hobbies.

## OpenAPI Specification

Below is the OpenAPI 3.1.0 specification for this API:

```yaml
openapi: 3.1.0
info:
  title: Eileen_Aylin API
  description: A personal overview of Eileen_Aylin, highlighting skills, interests, and hobbies.
  version: "1.0.0"
  contact:
    email: eileen.aylin@example.com
    url: https://eileenaylin.com
  license:
    name: MIT
    url: https://opensource.org/licenses/MIT
servers:
  - url: https://api.eileenaylin.com/v1
    description: Production server
  - url: https://sandbox.api.eileenaylin.com/v1
    description: Sandbox server for testing
paths:
  /about:
    get:
      summary: General Information
      description: Retrieve basic personal details about Eileen_Aylin.
      tags:
        - Personal Information
      responses:
        "200":
          description: Personal details retrieved successfully.
          content:
            application/json:
              schema:
                type: object
                properties:
                  name:
                    type: string
                    example: "@Eileen_Aylin"
                  year:
                    type: string
                    example: "Sophomore at CS"
        "404":
          description: Not found
          content:
            application/json:
              example:
                error: "Resource not found"
                message: "The requested resource does not exist."
  /interests:
    get:
      summary: Interests
      description: Retrieve a list of Eileen_Aylin's interests, categorized into IT-related and non-IT-related.
      tags:
        - Interests
      responses:
        "200":
          description: List of interests retrieved successfully.
          content:
            application/json:
              schema:
                type: object
                properties:
                  IT-related:
                    type: array
                    items:
                      type: string
                    example:
                      - "Coding in different languages"
                      - "App Development"
                  Non-IT-related:
                    type: array
                    items:
                      type: string
                    example:
                      - "Playing Guitar/Saz"
                      - "Badminton"
                      - "Bouldering"
                      - "Swimming"
                      - "Netflix"
        "500":
          description: Internal server error
          content:
            application/json:
              example:
                error: "Internal Server Error"
                message: "Something went wrong on the server."
  /skills:
    get:
      summary: Skills
      description: Retrieve a list of Eileen_Aylin's programming skills, frameworks, tools, and skills currently being learned.
      tags:
        - Skills
      responses:
        "200":
          description: List of skills retrieved successfully.
          content:
            application/json:
              schema:
                type: object
                properties:
                  programming_languages:
                    type: array
                    items:
                      type: string
                    example:
                      - "C"
                      - "Java"
                      - "Dart"
                      - "JavaScript"
                  frameworks:
                    type: array
                    items:
                      type: string
                    example:
                      - "Flutter"
                      - "Koa Framework"
                  tools:
                    type: array
                    items:
                      type: string
                    example:
                      - "Firebase"
                      - "Android Studio"
                      - "Xcode"
                      - "IntelliJ IDEA"
                      - "VS Code"
                  learning:
                    type: array
                    items:
                      type: string
                    example:
                      - "HTML"
                      - "CSS"
                      - "C++"
        "500":
          description: Internal server error
          content:
            application/json:
              example:
                error: "Internal Server Error"
                message: "Something went wrong on the server."
  /hobbies:
    get:
      summary: Hobbies
      description: Retrieve a list of Eileen_Aylin's hobbies, categorized into IT-related and non-IT-related.
      tags:
        - Hobbies
      responses:
        "200":
          description: List of hobbies retrieved successfully.
          content:
            application/json:
              schema:
                type: object
                properties:
                  IT-related:
                    type: array
                    items:
                      type: string
                    example:
                      - "Programming"
                      - "Backend/Frontend development"
                      - "APIs"
                      - "Flutter widgets"
                  Non-IT-related:
                    type: array
                    items:
                      type: string
                    example:
                      - "Playing Guitar/Saz"
                      - "Badminton"
                      - "Bouldering"
                      - "Swimming"
        "500":
          description: Internal server error
          content:
            application/json:
              example:
                error: "Internal Server Error"
                message: "Something went wrong on the server."
