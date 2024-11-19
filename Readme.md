# Java TCP Client-Server Application

## Introduction

This **Java TCP Client-Server Application** demonstrates a simple **file transfer mechanism** over a network. The client requests a file from the server, and the server sends the contents of the requested file back to the client. The system uses **TCP sockets** for communication, ensuring reliable, ordered, and error-free transmission.

---

## Prerequisites

Before running this application, ensure you have the following:

- **Java Development Kit (JDK)** installed on your computer.
- Basic understanding of **Java programming**.
- A **code editor** or integrated development environment (**IDE**) for Java.

---

## Usage

### Running the Server

1. Open a **terminal** or **command prompt**.

2. Navigate to the directory where the server code (`TCPS.java`) is located.

3. Compile the server code using the following command:

    ```bash
    javac TCPS.java
    ```

4. Run the server with the command:

    ```bash
    java TCPS
    ```

The server will listen for incoming client connections on **port 4000**. You can extend the server to handle multiple client connections or scale horizontally using **load balancers** and **auto-scaling** techniques in a cloud environment.

### Running the Client

1. Open another **terminal** or **command prompt**.

2. Navigate to the directory where the client code (`TCPC.java`) is located.

3. Compile the client code using the following command:

    ```bash
    javac TCPC.java
    ```

4. Run the client with the command:

    ```bash
    java TCPC
    ```

The client will prompt you to enter the filename you want to read. It establishes a TCP connection with the server, sends the filename, and receives the file contents.

---

## Future Enhancements

While this application is a basic demonstration, here are some simple improvements that could be made in the future:

1. **Error Handling**  
   - Add better error handling for cases when the file is not found or the connection is lost. This will help make the application more stable.

2. **Security**  
   - Implement basic security, such as ensuring that only authorized users can access the files.

3. **Multiple Clients**  
   - Allow the server to handle multiple clients at the same time, so that several people can request files simultaneously.

4. **File Compression**  
   - Add an option to compress files before sending them to improve transfer speed, especially for large files.

5. **Logging**  
   - Implement logging to track when files are requested, when errors happen, and to help with troubleshooting.
     
---

