# Cross-Platform-Story-Game-w-Flutter

-------------------------------------------------------
A P P L I C A T I O N   O V E R V I E W:
-------------------------------------------------------

Starting Project:

The idea of this project is a cross platform mobile game, with a Story that changes according to the user’s choices. In order for this project to come together, Dart was the programming language that was used, along with Flutter framework, and HIVE database. 



Environment (Language - Framework):

Dart is a programming language and Flutter is a mobile app development framework both created by Google in order to create high quality and responsive cross-platform Applications.
When building an app with Flutter, the Dart code is used to define the app's widgets, which are the building blocks of the app's user interface. These widgets are then rendered on the screen using Flutter's rendering engine.
The core of Flutter is the "widget tree," which is a hierarchy of widgets that define the layout and behaviour of the app. The framework provides a rich set of pre-built widgets that can be easily customised to create user interfaces.



Database:

HIVE is a data warehousing tool built on top of Hadoop that allows users to perform SQL-like queries on large datasets stored in the Hadoop Distributed File System (HDFS). 
When working with a CSV file, HIVE can be used to create a table that maps the columns in the CSV file to the corresponding fields in the HIVE table. This table can then be queried using SQL-like syntax to extract information from the data stored in the CSV file.
Once the data is loaded, you can use HIVE SQL to query the data in the table, just like you would with a relational database. HIVE also provides a number of built-in functions that can be used to perform data analysis and manipulation on the data stored in the table.



Application overview:

Both the design and the app I build  are simple.
Designwise, the application consists of a single page where the users can see the title of the game on top, The story line followed by the question that the user has to answer, and finally the two options.
Below all the text info, there are the option buttons and right underneath there is a reset button, that resets every text and option, to the beginning of the game. That way the users can play the game over and over again even if their character died in the game.
I didn’t go for anything extreme regarding colours and fonts. The background is a dark leaning coloured minimalist castle view. The font utilises Bold features, light colour that contrasts well the background, and it is big enough so even if the user has eyesight issues for any reason, they  can still interact with the game.
The story of the game is about a person that tries to escape a city. The user can choose between the two options provided to guide the plot of the game.

The way the app actually works with the help of HIVE database is:

1. User starts the app. -> Dart code converts to GUI with the help of Flutter SDK.
2. Dart code gets the Story, Question, and options info from the HIVE database table, which is created based on the CSV file (our ex dummy database).
3. Based on the user’s option (either OptionA or OptionB), each option has a unique ID that    corresponds to a unique record ID from the HIVE data table.
4. According to the record ID, the correct Story, Question and Options data appear.
5. Now if the user wants to reset the game, the RESET button can be used, which will set every bit of info displayed to the default (the beginning of the game).



-------------------------------------------------------
H O W   T O   R U N   T H E   A P P:
-------------------------------------------------------

1. Install Dart, Flutter, and Hive database on your machine.
2. Download the application zip file and etract it.
3. Check if everything is right with your IDE. If it require to download any additional packages, download them.
4. When the app is loaded into your IDE, open 'main.dart' file, and choose a device from the top right corner. (IntelliJ specific)
-if you are not using IntelliJ, search online how to setup a device for the IDE of your choice.-
5. After selecting the device you want the app to run on, click 'RUN' (in most IDEs is a green play button).

Congratulations! You can now run the game.
