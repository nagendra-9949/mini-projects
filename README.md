package seleniumwebdriver.SeleniumWebdriver; 
import java.util.ArrayList; 
import java.util.List; 
import java.util.NoSuchElementException; 
import java.util.Set; 
import java.util.concurrent.TimeUnit; 
import org.openqa.selenium.By; 
import org.openqa.selenium.JavascriptExecutor; 
import org.openqa.selenium.WebDriver; 
import org.openqa.selenium.WebElement; 
import org.openqa.selenium.chrome.ChromeDriver; 
import org.openqa.selenium.interactions.Actions; 
import org.openqa.selenium.support.ui.ExpectedConditions; 
import org.openqa.selenium.support.ui.Select; 
public class FirstTestClass { 
private static final String EC = null; 
public static void main(String[] args) { 
WebDriver driver = new ChromeDriver(); 
driver.manage().window().maximize(); 
driver.manage().timeouts().implicitlyWait(10, TimeUnit.SECONDS); 
driver.get("https://www.snapdeal.com");   
WebElement searchBox= driver.findElement(By.id("inputValEnter")); 
searchBox.sendKeys("kitchen product"); 
driver.findElement(By.xpath("//*[@id=\"sdHeader\"]/div[4]/div[2]/div/div[2]/button")).
 click(); 
driver.get("https://www.snapdeal.com/product/jisun-silver-stainless-steel
dish/646541758737"); 
try { 
Thread.sleep(5000); 
} catch (InterruptedException e) { 
e.printStackTrace(); 
} 
WebElement addToCart = driver.findElement(By.xpath("//*[@id=\"add-cart-button
id\"]")); 
addToCart.click(); 
try { 
Thread.sleep(5000); 
} catch (InterruptedException e) { 
e.printStackTrace(); 
} 
WebElement searchBox1 = driver.findElement(By.id("inputValEnter")); 
searchBox1.sendKeys("saree"); 
try { 
Thread.sleep(5000); 
} catch (InterruptedException e) { 
e.printStackTrace(); 
} 
driver.findElement(By.xpath("//*[@id=\"sdHeader\"]/div[4]/div[2]/div/div[2]/button")).
 click(); 
driver.get("https://www.snapdeal.com/product/rangita-navy-blue-banarasi
silk/667608902726"); 
try { 
       
       Thread.sleep(5000); 
   } catch (InterruptedException e) { 
     
       e.printStackTrace(); 
   } 
       
      WebElement pinCodeInput = driver.findElement(By.id("pincode-check")); // Update 
with correct ID or selector 
    
 
       
      pinCodeInput.sendKeys("560063");  
       
      try { 
           
          Thread.sleep(5000); 
      } catch (InterruptedException e) { 
        
          e.printStackTrace(); 
      } 
 
// Locate and click the "Check" button 
WebElement checkButton = driver.findElement(By.xpath("//*[@id=\"pincode
check-bttn\"]")); // Update with correct XPath 
checkButton.click(); 
try { 
Thread.sleep(5000); 
} catch (InterruptedException e) { 
e.printStackTrace(); 
} 
WebElement colorSwatch = driver.findElement(By.xpath("//*[@id=\"attribute
select-0\"]/div[2]/div/div/div[2]/div/div[1]/img")); // Replace with actual alt attribute 
value 
colorSwatch.click(); 
try { 
Thread.sleep(5000); 
} catch (InterruptedException e) { 
e.printStackTrace(); 
} 
WebElement addToCart1 = driver.findElement(By.xpath("//*[@id=\"add-cart
button-id\"]")); 
addToCart1.click(); 
try { 
Thread.sleep(5000); 
} catch (InterruptedException e) { 
e.printStackTrace(); 
} 
WebElement searchBox2 = driver.findElement(By.id("inputValEnter")); 
searchBox2.sendKeys("mens shirt"); 
try { 
Thread.sleep(5000); 
} catch (InterruptedException e) { 
e.printStackTrace(); 
} 
driver.findElement(By.xpath("//*[@id=\"sdHeader\"]/div[4]/div[2]/div/div[2]/button")).
 click(); 
driver.get("https://www.snapdeal.com/product/ivoc-olive-100-cotton
regular/678858533547#bcrumbSearch:mens%20shirt"); 
try { 
Thread.sleep(5000); 
} catch (InterruptedException e) { 
e.printStackTrace(); 
} 
WebElement sizeBox = driver.findElement(By.xpath("//*[@id=\"attribute-select
1\"]/div[2]/div/div/div[6]/div")); // Replace with actual XPath 
sizeBox.click(); 
try { 
Thread.sleep(5000); 
} catch (InterruptedException e) { 
e.printStackTrace(); 
} 
WebElement addToCart2 = driver.findElement(By.xpath("//*[@id=\"add-cart
button-id\"]")); 
addToCart2.click(); 
WebElement searchBox3 = driver.findElement(By.id("inputValEnter")); 
searchBox3.sendKeys("allen solly tshirt men"); 
try { 
Thread.sleep(5000); 
} catch (InterruptedException e) { 
e.printStackTrace(); 
} 
driver.findElement(By.xpath("//*[@id=\"sdHeader\"]/div[4]/div[2]/div/div[2]/button")).
 click(); 
WebElement highRatingReview = 
driver.findElement(By.xpath("//*[@id=\"content_wrapper\"]/div[7]/div[3]/div/div[1]/di
 v[2]/div[3]/div[3]/div/div[1]/label")); 
highRatingReview.click(); 
try { 
Thread.sleep(2000); 
} catch (InterruptedException e) { 
e.printStackTrace(); 
} 
JavascriptExecutor js = (JavascriptExecutor) driver; 
js.executeScript("window.scrollTo(0, 0);"); 
driver.get("https://www.snapdeal.com/search?keyword=allen%20solly%20tshirt%20me
 n&santizedKeyword=&catId=176&categoryId=0&suggested=true&vertical=&noOfRes
 ults=20&searchState=&clickSrc=suggested&lastKeyword=&prodCatId=&changeBack
 ToAll=false&foundInAll=false&categoryIdSearched=&cityPageUrl=&categoryUrl=&u
 rl=&utmContent=&dealDetail=&sort=rlvncy&q=avgRating%3A4.0%7CBrand%3A98
 %20Degree%20North%7C"); 
try { 
Thread.sleep(5000); 
} catch (InterruptedException e) { 
e.printStackTrace(); 
} 
driver.get("https://www.snapdeal.com/search?keyword=allen%20solly%20tshirt%20me
 n&santizedKeyword=&catId=176&categoryId=0&suggested=true&vertical=&noOfRes
 ults=20&searchState=&clickSrc=suggested&lastKeyword=&prodCatId=&changeBack
 ToAll=false&foundInAll=false&categoryIdSearched=&cityPageUrl=&categoryUrl=&u
 rl=&utmContent=&dealDetail=&sort=rlvncy&q=avgRating%3A4.0%7CBrand%3A98
 %20Degree%20North%7CColor_s%3ABlack%7C"); 
try { 
Thread.sleep(3000); 
} catch (InterruptedException e) { 
e.printStackTrace(); 
} 
driver.get("https://www.snapdeal.com/product/98-degree-north-polyester
regular/5764608158127556875#bcrumbSearch:allen%20solly%20tshirt%20men"); 
WebElement addToCart3 = driver.findElement(By.xpath("//*[@id=\"add-cart
button-id\"]")); 
addToCart3.click(); 
WebElement viewCart = 
driver.findElement(By.xpath("//*[@id=\"cartProductContainer\"]/div/div[2]/div[2]/div/d
 iv[2]/div")); 
viewCart.click(); 
try { 
Thread.sleep(5000); 
} catch (InterruptedException e) { 
e.printStackTrace(); 
} 
WebElement removeButton = 
driver.findElement(By.xpath("//*[@id=\"rtbScriptContainer\"]/div[5]/ul/li[3]/div[8]/div/
 span")); // Adjust index if needed 
removeButton.click(); 
try { 
Thread.sleep(5000); 
} catch (InterruptedException e) { 
e.printStackTrace(); 
} 
WebElement proceedtopay = driver.findElement(By.xpath("//*[@id=\"checkout
continue\"]/input[2]")); // Adjust index if needed 
proceedtopay.click(); 
WebElement emailInput = driver.findElement(By.xpath("//*[@id=\"username\"]")); 
emailInput.sendKeys("8546896606"); 
try { 
Thread.sleep(9000); 
} catch (InterruptedException e) { 
e.printStackTrace(); 
} 
WebElement continueButton = driver.findElement(By.id("login-continue")); 
continueButton.click(); 
WebElement code = driver.findElement(By.xpath("//*[@id=\"verification-code
val\"]")); 
code.sendKeys("1234"); 
         try { 
                
               Thread.sleep(8000); 
           } catch (InterruptedException e) { 
             
               e.printStackTrace(); 
           } 
         
         WebElement continueButton2 = 
driver.findElement(By.xpath("//*[@id=\"login-otp-submit\"]")); 
       continueButton2.click();      
       try { 
            
            Thread.sleep(5000); 
        } catch (InterruptedException e) { 
          
            e.printStackTrace(); 
        } 
 
 
       WebElement  resend_otp_button = 
driver.findElement(By.xpath("//*[@id=\"resend-OTP\"]/label[1]")); 
          resend_otp_button.click(); 
        try { 
             
            Thread.sleep(15000); 
        } catch (InterruptedException e) { 
          
            e.printStackTrace(); 
        } 
           
         WebElement continueButton3= 
driver.findElement(By.xpath("//*[@id=\"login-otp-submit\"]")); 
         continueButton2.click();     
         resend_otp_button.click(); 
      try { 
          
            Thread.sleep(20000); 
        } catch (InterruptedException e) { 
          
            e.printStackTrace(); 
        } 
         driver.get("https://www.snapdeal.com/product/ivoc-olive-100-cotton
regular/678858533547"); 
         WebElement addToCart4= driver.findElement(By.xpath("//*[@id=\"add-cart
button-id\"]")); 
addToCart4.click(); 
WebElement 
ProceedToCheckout=driver.findElement(By.xpath("//*[@id=\"cartProductContainer\"]/
 div/div[2]/div[2]/div/div[2]/a")); 
ProceedToCheckout.click(); 
WebElement Name=driver.findElement(By.name("fullName")); 
Name.sendKeys("Bhavadarani V"); 
WebElement Address=driver.findElement(By.xpath("//*[@id=\"address\"]")); 
Address.sendKeys("SVCE KIA ROAD Bengaluru"); 
WebElement AddressType=driver.findElement(By.xpath("//*[@id=\"shipping
address-form\"]/div/div[10]/div/div[1]")); 
AddressType.click(); 
try { 
Thread.sleep(15000); 
} catch (InterruptedException e) { 
e.printStackTrace(); 
} 
WebElement 
SaveandContinue=driver.findElement(By.xpath("//*[@id=\"delivery-modes
continue\"]/span")); 
SaveandContinue.click(); 
         try { 
            
             Thread.sleep(5000); 
         } catch (InterruptedException e) { 
           
             e.printStackTrace(); 
         } 
          
         WebElement Proceedtopay1=driver.findElement(By.xpath("//*[@id=\"make
payment\"]")); 
         Proceedtopay1.click(); 
          
         try { 
              
          Thread.sleep(5000); 
      } catch (InterruptedException e) { 
        
          e.printStackTrace(); 
      } 
          
         driver.quit(); 
 } 
}
