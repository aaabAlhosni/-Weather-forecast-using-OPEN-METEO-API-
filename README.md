=========================================================
TRAINING LOG: API CONSUMPTION & JAVA INTEGRATION
=========================================================

1. INTRODUCTION: WHAT I WILL DO
---------------------------------------------------------
In this session, I will demonstrate the full lifecycle of consuming a REST API. 
My objective is to retrieve real-time weather data for Tokyo from the 
Open-Meteo public API. 

I will move from manual verification in a GUI client to automated execution 
in a Java environment. Specifically, I will:
- Establish a connection to a live endpoint.
- Analyze the structure of HTTP responses.
- Conduct error-handling tests.
- Implement a programmatic solution using the UniRest library.

2. STEP-BY-STEP WORKFLOW
---------------------------------------------------------
To complete this task, I will use the following software:
- Postman (API Client)
- Java IDE (IntelliJ, Eclipse, or VS Code)
- UniRest Library (Maven/Gradle dependency)

STEP 1: INITIAL REQUEST CONFIGURATION
- I will open Postman and create a new GET request.
- I will target the following URL:
  https://api.open-meteo.com/v1/forecast?latitude=35&longitude=139&current_weather=true
- I will manually add a "Content-Type: application/json" header to define the 
  data format for the session.

STEP 2: RESPONSE ANALYSIS
- I will click 'Send' and inspect the response.
- I will verify that the status code is 200 (Success).
- I will examine the JSON structure to locate the 'current_weather' object.

STEP 3: NEGATIVE TESTING (VALIDATION)
- I will intentionally break the request by changing the latitude to "INVALID".
- I will confirm that the system returns a 4xx error code, proving that I 
  can identify and handle client-side input errors.

STEP 4: JAVA UNIREST IMPLEMENTATION
- I will use Postman's code generation tool to extract the Java UniRest snippet.
- I will implement the necessary logic in my Java project to parse and handle 
  the response body.

3. EXPECTED OUTPUT
---------------------------------------------------------
By the end of this process, I will have achieved the following:
- A verified API call history in Postman.
- A functional Java class that retrieves and prints live weather data.
- A clear understanding of the three response components: Status, Headers, and Body.
- The ability to differentiate between a successful 'Read' operation (GET) 
  and a handled error scenario.

=========================================================
END OF LOG
=========================================================
