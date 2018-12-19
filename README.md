# Se-Custom-Xpath

package SeleniumSession;

import java.util.concurrent.TimeUnit;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;

public class CustomXpath {

	public static void main(String[] args) {
		
		System.setProperty("webdriver.chrome.driver", "C:\\Users\\Arun\\eclipse-workspace\\Selenium\\lib\\chromedrivers\\chromedriver.exe");
		WebDriver driver = new ChromeDriver();
		
		driver.manage().window().maximize();
		
		
		
		driver.manage().timeouts().pageLoadTimeout(40, TimeUnit.SECONDS);
		driver.manage().timeouts().implicitlyWait(30, TimeUnit.SECONDS);
		
		driver.get("https://www.ebay.com/");
		
		//driver.findElement(By.xpath("//*[@id=\"gh-ac\"]")).sendKeys("java");
		
		//driver.findElement(By.xpath("//input[@type='text']")).sendKeys("Java");
		
		//driver.findElement(By.xpath("//input[@placeholder='Search for anything']")).sendKeys("Automation");
		
		//driver.findElement(By.xpath("//input[@class='gh-tb ui-autocomplete-input ui-autocomplete-loading']")).sendKeys("javaaa");
		
		//driver.findElement(By.xpath("//input[contains(@type,'text')]")).sendKeys("autonomous"); // DYNAMIC ID HANDLING
		
		//driver.findElement(By.xpath("//input[contains(@id,'gh-')]")).sendKeys("autonomoues");
		
		//driver.findElement(By.xpath("//input[starts-with(@id,'gh-')]")).sendKeys("python");
		
		
		//for links:
		//all links are represented by <a> html tag.
		driver.findElement(By.xpath("//a[contains(text(),'Sign in')]")).click();
		
		
		
		
		
		
			
		//*[@id="gh-ac"]
		//<input type="text" class="gh-tb ui-autocomplete-input ui-autocomplete-loading" size="50" maxlength="300" placeholder="Search for anything" id="gh-ac" name="_nkw" autocapitalize="off" autocorrect="off" spellcheck="false" autocomplete="off" aria-haspopup="true" role="combobox" aria-owns="ui-id-1">

	}

}
