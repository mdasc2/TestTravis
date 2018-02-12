package Test;

import javafx.event.ActionEvent;
import javafx.fxml.FXML;
import javafx.scene.control.Button;
import javafx.scene.control.TextField;

public class CalculatorController 
{

	@FXML
	private TextField numOne = new TextField();
	@FXML
	private TextField numTwo = new TextField();
	
	@FXML
	private TextField equals = new TextField();
	
	@FXML
	private Button minusButton = new Button();	
	@FXML
	private Button plusButton = new Button();
	@FXML
	private Button multiButton = new Button();
	@FXML
	private Button divButton = new Button();
	
	
	@FXML
	public void Multiply(ActionEvent event)
	{
		int num2 = Integer.parseInt(numTwo.getText());
		int num1 = Integer.parseInt(numOne.getText());
		
		equals.setText(Integer.toString(num1 * num2));	
	}
	@FXML
	public void Add(ActionEvent event)
	{
		int num2 = Integer.parseInt(numTwo.getText());
		int num1 = Integer.parseInt(numOne.getText());
		
		equals.setText(Integer.toString(num1 + num2));
		
	}
	@FXML
	public void Subtract(ActionEvent event)
	{
		int num2 = Integer.parseInt(numTwo.getText());
		int num1 = Integer.parseInt(numOne.getText());
		equals.setText(Integer.toString(num1 - num2));
	}
	@FXML
	public void Divide(ActionEvent event)
	{
		int num2 = Integer.parseInt(numTwo.getText());
		int num1 = Integer.parseInt(numOne.getText());
		
		equals.setText(Integer.toString(num1 / num2));
	}

}
