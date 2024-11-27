< openapi: 3.1.0
info:
  title: Eileen_Aylin API
  description: A personal overview of Eileen_Aylin, highlighting skills, interests, and hobbies.
  version: "1.0.0"
paths:
  /about:
    get:
      summary: General Information
      description: Retrieve basic personal details.
      responses:
        "200":
          description: Personal details retrieved successfully.
          content:
            application/json:
              example:
                name: "@Eileen_Aylin"
                year: "Sophomore at CS"
  /interests:
    get:
      summary: Interests
      description: Retrieve a list of interests.
      responses:
        "200":
          description: List of interests retrieved successfully.
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
      summary: Skills
      description: Retrieve a list of programming skills, frameworks, and tools.
      responses:
        "200":
          description: List of skills retrieved successfully.
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
      summary: Hobbies
      description: Retrieve a list of hobbies, both IT-related and non-IT-related.
      responses:
        "200":
          description: List of hobbies retrieved successfully.
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
                  - "Swimming" >
