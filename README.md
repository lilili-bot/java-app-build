# Java Application Build and Run Guide

## Prerequisites

Ensure that you have the following installed on your system:

1. **Java Development Kit (JDK) 17** or later
2. **Gradle** (If not installed, you can use the Gradle wrapper provided in the project)

## Building the Application

First, you need to build the application using Gradle. This will compile the code and package it into a JAR file.

### Steps to Build

1. Open a terminal or command prompt.
2. Navigate to the root directory of your project.
3. Run the following command to build the project:

    ```sh
    ./gradlew build   # For macOS/Linux
    gradlew build     # For Windows
    ```

    This will execute the `build` task and produce a JAR file in the `build/libs` directory.

## Running the Application

After building the project, you can run the application using the generated JAR file.

### Steps to Run

1. In the terminal or command prompt, navigate to the `build/libs` directory:

    ```sh
    cd build/libs
    ```

2. Run the JAR file using the `java -jar` command:

    ```sh
    java -jar java-app-build-1.0-SNAPSHOT.jar
    ```

    Make sure to replace `java-app-build-1.0-SNAPSHOT.jar` with the actual name of the JAR file generated in the `build/libs` directory if it differs.

## Example

Here is an example of the entire process:

1. **Build the project**:

    ```sh
    ./gradlew build
    ```

2. **Navigate to the `build/libs` directory**:

    ```sh
    cd build/libs
    ```

3. **Run the application**:

    ```sh
    java -jar java-app-build-1.0-SNAPSHOT.jar
    ```

## Troubleshooting

- **JAVA_HOME is not set**: Ensure the `JAVA_HOME` environment variable is set to the JDK installation directory.
- **Build errors**: Check the terminal output for any errors during the build process. Ensure all dependencies are correctly specified in `build.gradle`.
- **JAR not found**: Ensure you are in the `build/libs` directory and that the build process completed successfully.

For further details and advanced configurations, refer to the official [Gradle documentation](https://docs.gradle.org/current/userguide/userguide.html) and [Java documentation](https://docs.oracle.com/en/java/).

---

Feel free to reach out for further assistance or if you encounter any issues during the setup process.
