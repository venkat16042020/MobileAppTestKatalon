npm install appium
set APPIUM_HOME in environment variables: C:\Users\venkat\AppData\Roaming\npm\node_modules\appium
add path with : C:\Users\venkat.kamani\AppData\Roaming\npm    this is to get appium executable file.
C:\Users\VENKAT~1.KAM\AppData\Roaming\npm\node_modules\appium>appium driver install uiautomator2
where appium
install android studio for device manager to have emulators.

Start recording the mobile test in katlon studio.
It would select the emulator form AndroidStudioDeviceManage.
start recording it.
create your script.
run the script.
script gets created in keyword view. we can see the script in script view also.
sample is here:
==================================================
import static com.kms.katalon.core.checkpoint.CheckpointFactory.findCheckpoint
import static com.kms.katalon.core.testcase.TestCaseFactory.findTestCase
import static com.kms.katalon.core.testdata.TestDataFactory.findTestData
import static com.kms.katalon.core.testobject.ObjectRepository.findTestObject
import static com.kms.katalon.core.testobject.ObjectRepository.findWindowsObject
import com.kms.katalon.core.checkpoint.Checkpoint as Checkpoint
import com.kms.katalon.core.cucumber.keyword.CucumberBuiltinKeywords as CucumberKW
import com.kms.katalon.core.mobile.keyword.MobileBuiltInKeywords as Mobile
import com.kms.katalon.core.model.FailureHandling as FailureHandling
import com.kms.katalon.core.testcase.TestCase as TestCase
import com.kms.katalon.core.testdata.TestData as TestData
import com.kms.katalon.core.testng.keyword.TestNGBuiltinKeywords as TestNGKW
import com.kms.katalon.core.testobject.TestObject as TestObject
import com.kms.katalon.core.webservice.keyword.WSBuiltInKeywords as WS
import com.kms.katalon.core.webui.keyword.WebUiBuiltInKeywords as WebUI
import com.kms.katalon.core.windows.keyword.WindowsBuiltinKeywords as Windows
import internal.GlobalVariable as GlobalVariable
import org.openqa.selenium.Keys as Keys

Mobile.startApplication('C:\\Users\\venkat.kamani\\Downloads\\ApiDemos-debug.apk', true)

Mobile.tap(findTestObject('Object Repository/android.widget.TextView - Text'), 0)

Mobile.tap(findTestObject('Object Repository/android.widget.TextView - LogTextBox'), 0)

Mobile.setText(findTestObject('Object Repository/android.widget.TextView'), 'kkkkkkkkkk', 0)

Mobile.getText(findTestObject('Object Repository/android.widget.TextView - TextLogTextBox'), 0)

Mobile.getText(findTestObject('Object Repository/android.widget.TextView'), 0)

Mobile.closeApplication()

=====================================================
