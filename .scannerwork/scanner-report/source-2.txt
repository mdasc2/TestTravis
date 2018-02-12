package Test;

import java.io.IOException;

import javafx.application.Application;
import javafx.event.ActionEvent;
import javafx.stage.Stage;
import javafx.fxml.FXML;
import javafx.fxml.FXMLLoader;
import javafx.scene.Parent;
import javafx.scene.Scene;
import javafx.scene.control.Button;
import javafx.scene.control.TextField;

public class Calculador extends Application {

	@Override
	public void start(Stage primaryStage) throws IOException 
	{
		CalculatorController cc = new CalculatorController();
		FXMLLoader loader = new FXMLLoader();
		loader.setLocation(getClass().getResource("/Test/JavaFX.fxml"));
		loader.setController(cc);
		
		Parent root = (Parent) loader.load();
		Scene scene = new Scene(root);
		primaryStage.setScene(scene);
		primaryStage.show();
	}

	public static void main(String[] args) {
		launch(args);
	}
}
