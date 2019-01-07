package com.effectivetesting.sanity;

import java.util.concurrent.TimeUnit;

import org.junit.After;
import org.junit.Before;
import org.junit.Test;
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;
import org.openqa.selenium.support.ui.ExpectedConditions;
import org.openqa.selenium.support.ui.Select;
import org.openqa.selenium.support.ui.WebDriverWait;

public class TestSimulacionAn {
	
private WebDriver driver;
	
	@Before
	public void setUp() {
		System.setProperty("webdriver.chrome.driver", "C:\\ChromeDriver\\chromedriver.exe");
		driver = new ChromeDriver();
		driver.manage().timeouts().implicitlyWait(10, TimeUnit.SECONDS);
		driver.get("http://190.216.52.100/pvendedor/");
		driver.findElement(By.id("inputLogin")).sendKeys("1000001");
		driver.findElement(By.id("inputPassword")).sendKeys("01230123");
		driver.findElement(By.id("continue")).click();
		driver.manage().timeouts().implicitlyWait(3, TimeUnit.SECONDS);
		driver.findElement(By.xpath("/html/body/section[2]/div/div/div[1]/h2/b")).getText();
		driver.findElement(By.xpath("/html/body/header/nav/div[2]/ul[1]/li[1]/a")).click();
		driver.findElement(By.xpath("/html/body/header/nav/div[2]/ul[1]/li[1]/ul/li[1]/a")).click();
		driver.findElement(By.xpath("//*[@id=\"headingOne\"]/a/h4")).click();
		driver.findElement(By.id("button360802")).click();
		WebElement element = (new WebDriverWait(driver, 10))
		   .until(ExpectedConditions.elementToBeClickable(By.id("precio")));
		element.sendKeys("980000");

		driver.findElement(By.xpath("//*[@id=\"formSelect\"]/section/div/div/div[3]/div/div[2]/button[1]")).click();
		}
	
	@Test
	public void TestFinanciacionAn () 
	
	 {
		new Select(driver.findElement(By.xpath("//*[@id=\"lineas1\"]/option[6]")));
		
		
		
		}

	
	
	

		
		
		
	
	
	@After
	public void tearDown() {
//		driver.quit();
	}
	