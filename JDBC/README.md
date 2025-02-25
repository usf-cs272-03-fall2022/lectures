Java Database Connectivity (JDBC)
=================================================

These demos illustrate basic concepts related to embedded Jetty and embedded Jetty and database connections using JDBC in Java.

## Lecture Resources

The following archived recordings of the lecture code may be useful:

  - [JDBC](https://docs.google.com/presentation/d/e/2PACX-1vT7nGgdwQx2Vqj6vSAgEi3CTK2dEQmbq_Xf6dcnc4UWVPuzwwZg5_bWz3n2P5L3stqddAzY5BtAE2e4/pub?start=false&loop=false&delayms=3000) ([Video](https://drive.google.com/file/d/1bgEAcSx7OhRRziOo8MsiP_DjcrOrhClG/view?usp=sharing))
  
The following archived recordings of the lecture code may be useful:

  - [Faculty Server Part 1 - Demo, HTML, and SQL](https://drive.google.com/file/d/1Q8jyBIsugwjbzk-JGJJZT5QF4EvAs-xN/view?usp=sharing)
  - [Faculty Server Part 2 - DatabaseConnector.java](https://drive.google.com/file/d/1nJ17EatO7ZeureUORtqDLfTaw6MXyIZj/view?usp=sharing)
  - [Faculty Server Part 3 - FacultyServer.java](https://drive.google.com/file/d/1yqeeCTD2j3qKz6Q_7sWn94SYkAV18_lt/view?usp=sharing)
  - [Faculty Server Part 4 - FacultyServlet.java](https://drive.google.com/file/d/1J-buaf3BIVp4QYYm6u8M6-fzN_tXT3as/view?usp=sharing)

The recording transcripts are autogenerated. The recordings may differ slightly from the latest version of the associated slides and code.

### Configuration

Modify `database.properties` with your MariaDB username and password. Create an SSH tunnel to forward anything sent to your
port 3307 to our on-campus MariaDB database server port 3306 using this command:

```
ssh username@stargate.cs.usfca.edu -L 3307:sql.cs.usfca.edu:3306
```

...where `username` is your CS username. You will be prompted for your CS password.

If you are a Mac user, you can create a `tunnel.command` file with the SSH command you should use and give the file execute privileges. Then, you should be able to double-click the file to run the command.

If you are a Windows user, you can use Windows Terminal to setup the tunnel (or port forwarding) or use a program like Putty. (Search for "Putty Port Forwarding" to find several guides.)

### Security Notes

Nothing we do regarding security will be effective unless we also use encrypted communication between the client browser and the web server. For this, you should be using HTTPS instead of HTTP.

Unless you are a security expert, I always recommend you use a package designed by security professionals for handling sensitive information (like username and passwords). However, there are some best practices guides out there. See the [OWASP Password Storage Cheat Sheet](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Password_Storage_Cheat_Sheet.md) for an example.

## Official Resources

The following official [Java Tutorials](http://docs.oracle.com/javase/tutorial/index.html) may be useful:

  - [The Java Tutorials – Lesson: JDBC Basics](https://docs.oracle.com/javase/tutorial/jdbc/basics/index.html)

