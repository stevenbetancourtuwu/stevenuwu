package application;

import javafx.application.Application;
import javafx.scene.Scene;
import javafx.scene.control.*;
import javafx.scene.layout.GridPane;
import javafx.stage.Stage;

public class Main extends Application {

    @Override
    public void start(Stage primaryStage) {
        primaryStage.setTitle("allControls.fxml");

        GridPane grid = new GridPane();
        grid.setVgap(10);
        grid.setHgap(10);

        // Button
        Button button = new Button("Button");
        grid.add(new Label("Button:"), 0, 0);
        grid.add(button, 1, 0);

        // CheckBox
        CheckBox checkBox = new CheckBox("CheckBox");
        grid.add(new Label("CheckBox:"), 0, 1);
        grid.add(checkBox, 1, 1);

        // Hyperlink
        Hyperlink hyperlink = new Hyperlink("Hyperlink");
        grid.add(new Label("Hyperlink:"), 0, 2);
        grid.add(hyperlink, 1, 2);

        // ToggleButton
        ToggleButton toggleButton = new ToggleButton("ToggleButton");
        grid.add(new Label("ToggleButton:"), 0, 3);
        grid.add(toggleButton, 1, 3);

        // RadioButton
        RadioButton radioButton = new RadioButton("RadioButton");
        grid.add(new Label("RadioButton:"), 0, 4);
        grid.add(radioButton, 1, 4);

        // Label
        Label label = new Label("Label");
        grid.add(new Label("Label:"), 0, 5);
        grid.add(label, 1, 5);

        // TextField
        TextField textField = new TextField("some text...");
        grid.add(new Label("TextField:"), 0, 6);
        grid.add(textField, 1, 6);

        // PasswordField
        PasswordField passwordField = new PasswordField();
        passwordField.setText("password");
        grid.add(new Label("PasswordField:"), 0, 7);
        grid.add(passwordField, 1, 7);

        // TextArea
        TextArea textArea = new TextArea("This is very long text that will wrap to several lines.");
        textArea.setWrapText(true);
        grid.add(new Label("TextArea:"), 0, 8);
        grid.add(textArea, 1, 8);

        // ProgressIndicator
        ProgressIndicator progressIndicator = new ProgressIndicator(0.49);
        grid.add(new Label("ProgressIndicator:"), 0, 9);
        grid.add(progressIndicator, 1, 9);

        // ProgressBar
        ProgressBar progressBar = new ProgressBar(0.49);
        grid.add(new Label("ProgressBar:"), 0, 10);
        grid.add(progressBar, 1, 10);

        // Slider
        Slider slider = new Slider();
        grid.add(new Label("Slider:"), 0, 11);
        grid.add(slider, 1, 11);

        Scene scene = new Scene(grid, 400, 500);
        primaryStage.setScene(scene);
        primaryStage.show();
    }

    public static void main(String[] args) {
        launch(args);
    }
}

![image](https://github.com/stevenbetancourtuwu/stevenuwu/assets/172458170/81dac05d-f0a7-47c9-a653-5521754d292e)
