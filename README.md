# App.VWO
package com.fb;
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;
import java.util.Scanner;
public class AppVwo {

	public static void main(String[] args) throws InterruptedException
	{

		WebDriver driver=new ChromeDriver();
		
		
		driver.get("https://vwo.com/free-trial/?utm_medium=website&utm_source=login-page&utm_campaign=mof_eg_loginpage");
		driver.manage().window().maximize();
		driver.findElement(By.xpath("//input[@id='page-v1-step1-email']")).sendKeys("ksharbon782@gmail.com");
		driver.findElement(By.xpath("//input[@id='page-945cu-gdpr-consent-checkbox']")).click();
		driver.findElement(By.xpath("//button[normalize-space()='Create a Free Trial Account']")).click();
		Thread.sleep(10000);
		driver.findElement(By.xpath("//input[@id='page-v1-fname']")).sendKeys("Mosharof");
		driver.findElement(By.xpath("//input[@id='page-v1-lname']")).sendKeys("Hossain");
		driver.findElement(By.xpath("//input[@id='page-v1-pnumber']")).sendKeys("560665201");
		Thread.sleep(2000);
		driver.findElement(By.xpath("//input[@id='page-v1-pwd']")).sendKeys("Mosharof1@");
		
		driver.findElement(By.xpath("//*[@id=\"page-free-trial-signup-form-step2\"]/div[2]/div[4]/div[1]/div[1]/label/input")).click();
		driver.findElement(By.xpath("//*[@id=\"page-free-trial-signup-form-step2\"]/div[2]/div[5]/div/div/div[1]/label/input")).click();
		driver.findElement(By.xpath("//button[normalize-space()='Create Account']")).click();
				
	}

	
	
}
