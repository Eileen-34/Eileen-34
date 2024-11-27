openapi: 3.1.0
info:
  title: Eileen_Aylin API
  description: Personal and Professional Overview of Eileen_Aylin
  version: "1.0.0"
paths:
  /about:
    get:
      summary: Retrieve general information
      responses:
        "200":
          description: General Information
          content:
            application/json:
              example:
                name: "@Eileen_Aylin"
                year: "Sophomore at CS"
  /interests:
    get:
      summary: Retrieve interests
      responses:
        "200":
          description: List of Interests
          content:
            application/json:
              example:
                IT-related: 
                  - "Coding in different languages"
                  - "App Development"
                Non-IT-related: 
                  - "Playing Guitar/Saz"
                  - "Badminton"
                  - "Bouldering"
                  - "Swimming"
                  - "Netflix"
  /skills:
    get:
      summary: Retrieve skills
      responses:
        "200":
          description: List of Skills
          content:
            application/json:
              example:
                programming_languages:
                  - "C"
                  - "Java"
                  - "Dart"
                  - "JavaScript"
                frameworks:
                  - "Flutter"
                  - "Koa Framework"
                tools:
                  - "Firebase"
                  - "Android Studio"
                  - "Xcode"
                  - "IntelliJ IDEA"
                  - "VS Code"
  /hobbies:
    get:
      summary: Retrieve hobbies
      responses:
        "200":
          description: List of Hobbies
          content:
            application/json:
              example:
                IT-related:
                  - "Programming"
                  - "Backend/Frontend development"
                  - "APIs"
                  - "Flutter widgets"
                Non-IT-related:
                  - "Playing Guitar/Saz"
                  - "Badminton"
                  - "Bouldering"
                  - "Swimming"
