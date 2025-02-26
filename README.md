// Demonstrating a basic JavaFX application //

package com.example.hw_1;

import javafx.application.Application;
import javafx.scene.Group;
import javafx.scene.Scene;
import javafx.scene.paint.Color;
import javafx.scene.text.Text;
import javafx.stage.Stage;
public class HelloJavaFX extends Application{
    //--------------------------------------------------------------------
// Creates and displays three Text objects in a JavaFX window.
//--------------------------------------------------------------------
    public void start(Stage primaryStage)
    {
        Text name = new Text(30, 20, "Name: Rifat Ibrahim");
        Text major = new Text(30, 40, "Major: Information Technology");
        Text email = new Text(30, 60, "University email: ibrahimr8@montclair.edu");
        Group root = new Group(name,major,email);
        Scene scene = new Scene(root, 300, 200, Color.ANTIQUEWHITE);

        primaryStage.setTitle("Student Information");
        primaryStage.setScene(scene);
        primaryStage.show();
    }

    // Launches the JavaFX application after inputting Text objects //
    public static void main(String[] args)
    {
        launch(args);
    }
}
