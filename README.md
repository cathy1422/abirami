package khan;

import org.openqa.selenium.chrome.ChromeDriver;
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;


public class academy {

	public static void main(String[] args) throws InterruptedException {
		WebDriver Math= new ChromeDriver();
		Math.get("https://testsheepnz.github.io/BasicCalculator.html");
		
		WebElement course=Math.findElement(By.id("number1Field"));
		course.sendKeys("14");
		
		WebElement course1 =Math.findElement(By.id("number2Field"));
		course1.sendKeys("15");
		
		WebElement course2 =Math.findElement(By.id("calculateButton"));
		course2.click();

		WebElement link =Math.findElement(By.linkText("About"));
		String Hyperlink= link.getText();
		 System.out.println("the link is "+ Hyperlink);
		 Thread.sleep(2000);
		 
		 
		 Math.close();
		 
		 
		 
		
		
		
		
	
		
		}

	}


