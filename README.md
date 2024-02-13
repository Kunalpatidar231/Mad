1.Create "Hello World" application - That will display" Hello World" In the middle of the screen in the red color with white background.
Activity _main. Xml
< ?xml version = "1.0" encoding = "Utf-8"?>
XmIns: app=" http://schemas. android-com/apk/res -auto"
xmens: tools = "http: // schemas. android. com)toots"
android: layout -width: "match-parent"
android: layout - height = " match_ parent"
tools: context = ".MainActivity">
< TextView
android: layout _width = Wrap-content"
andrid: layout height. " a-cantent"
android: textcolor = "#FF0000"
appi layout constraint Bottom toBottom of= "parent"
app: layout constraint left -toleftof = "parent"
app: layout constraintRight_ toRightof = "parent"
app: layout - constraint Top-toTapo = "parent"/>
</android X. constraint layout. widget. Constraint Layout >

➡️Main Activity. Java package com. example. helloworla;
import android suppost V7 app. AppcompatActivity , import android. os. Bundle>
public class MainActivity extends ApplompatActivity E
@override
protected void on Create (Bundle saved InstanceStael super-Oncreate (Saved Instancestate);
SetContentviero (R-dayout.activity-main);

2. Create Myinto application. That will display your name, qualificatio Contact num, email id and gray All Using Java code. address with background must have different color of above program
Ans XML dayout:-
<?xml version="1.0" encoding="utf-8"?>
<Relative dayout xmlns:android="http://schema.android.com/
apk/res/android" android: layout-width="match-parent"
android:layout- height="match-parent" android: background="#808080">
<TextView
android:id="@+id/nameTextview" android:layout width="wrap-content"
1: layout height="wrap-content" android: android :text="Your name" android: text color="#FFFFFF"
android:layout marginTop = "20dp"/>
<TextView
android:id="@+id/qualificationTextView" android:layout-width="wrap-content" android: layout-height="wrap-content" Your Qualification" android: text = " You android: textcolor="#00FF00" android:layout below = "@id /name Textview" android:layout-marginTop = "20dp" />

< Textview
android: id = "@t id/contactTextview "
android: Layout-Width= " wrap- content" andrais: leyout height " wrap cartent"
android: textcolor = "#FF0000"
android: Layout-below="@*id /qualificationTextview"
androld: layout _margin Top = "2020"/>
< Textview
android: id = "@+ id / email Textview"
android: layout _Width= " wrap -content" android: ayout height "irap-Content" android: textcolor= "#0000FF"
android: dayout-below="@* id / contactextview"
android: layout-margintop = "20dp"/>
< TextView
android: id= "
@+ id / addressText View"
android: textolor = "#FEFF00"
androld: Layout -below = "@id /email Textviero"
android: dayaut marginTop = "202p"/>
</Relativedayout >


➡️Java
import android • graphics. color; import android. as - Bundle; import android • widget. TextVieo;
import androids. applompat•app.AppcompatActivity;
public Class Your InFoActivity extends Applompat Activity é @ override
protected Vold on reate Bundle savedinstance state) f super. on (reate (saved Instance State ); setcontentView (R. layout. activity -your-info);
Textvier nameTextriew: FindViewbyIa (R•id-nameTextview);
Text vier qualification TextView= Findview ByTa (R• id• qualificationText viaw);
Textview contact Textview = find ViewById (R. id. contactTextview);
Textview email Textview = find view By Id (Rid. a emailTextview);
Textview addresstextview= tindVierBy Id (R.id- addresstextvier);
hame Textview. settextolor (10/or-BLUE);
qualitication Textview - setTextLolor (Color GREEN); contact Textvie. SetTextcolor (color.RED); email Text view • set Textcolor (color. YELLOW); address Text view. settext Color (color.CYAN);

3 Write A program to demonstrate life cycle of activity in android
Ans
XML code:-
<?xml version="1.0" encoding="utf-8"?>
<linearLayout xmlns:android="http://schemas.android.com/ apk/res/android"
android:layout-width="match-parent" android: dayout-height="match-parent"
android: orientation="vertical"
android: padding = "16 dp">
<TextView
android:layout-width="wrap-content" android: Layout - height= "wrap-content"
android : text = si Hello, Activity Life cycle!" android: textsize = "18sp"/>
</ linear layout>

➡️JAVA code
A
import android.app.Activity; import android.os.Bundle;
Import android.util.Log;
public class MainActivity extends Activity {
private static final string TAG = "ActivityLite Cycle";
@override
protected void onCreate(Bundle savedInstanceState) { super.onCreate (savedInstanceState) setContentView(R.layout.activity.main); dogd (TAG, "onCreate");
override
protected void onStart(){
super.onStart(); Log.d (TAG, "onstart");
@override
protected void on Resume () {
super onResume();"); Log'd (TAG, "onResume");
@override
protected void on Pause() { Super.onPause(); Log.d(TAG, "onPause");
@override
protected void on stop() {

super-onstop();
dog. d (TAr, "onstop");
У
@override
protected void onDestroy 0)E super. on Destroy () ;
dog-d (TAG, " onDestroy");
У
•@override
Restart
protected void onResume ()S
super. on Restart (); dogid (TAG, " onRestart");
}
}

4.
Ans
Pg. No.:..
Date :.
reate An Application that designs a layout with a text Box and Button named submit. Ihe user should enter the text in the text Box. When the submit button is clicked than the text in the text box should be displayed in the toast.
XML code :-
≤? xme version ="1-0" encoding = "utt - 8"?>
< lineardayout xmens: android = "http:// schemas.andraid.com/
apk/ res/ android"
android: layout width = " match, parent"
android: layout-height=" match-parent
android : orientation = Vertical"
android: padding = "16dp".
<editText
android: id = "@+id /editText"
android: layout _width = " match _pasent"
android: Layout _ height = "wrap - content"
android: hint = " Enter text"/ >
Button
andraid: id = "At id/ submitBtn"
android: Layout width = " wrap -content"
android: dayout _height = " wrap-content"
aundroid: text = "Submit" />
</lineardayout >


➡️JAVA CODE
import android 0s. Bundes
impost android. viero. Vier; import android • widget - Button; import android. widget. EditText; impos android. widget - Toast; import androidx. appcompat - app•App compatActivity; public(lass MainActivity extends App compat Activity E
@override
protected void onCreate (Bundle saved Instance state ) E super. ontreate (saved Instance state);
SetcontentView (Rolayout.activity_main) ;
final EditText edittext = findView ByTa (R.id• editText);
Button submitBtn=tindVieByID (R•id - SubmitBtn);
SubmitBtn •SetonlicKlistener (new View. Onclicklistener() { @override
public void ondlick(viao vier)s
string enteredTeXt = editText.getText () • tostring ;
it (lentered Text. (SEmpty() [
show Toast (" Entered Text: "+ enteredText);
y else E
SKaL ast （please enter text bebre submiting"）3
3) ;
子
private Void show Toast (String message E
Toast. make tag Text (this, message, ToasT. LENGTH- SHORT •Show));
}
}

5.
Create An android Application named "Arithmetic-op" which perform all basic arithmetic operation like addition, substractis, multiplication and division.
XML Code:-
Ans
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com /apk/res/android" xmens: tools="http://schemas.android.com/tools" width="match.parent" android:layout-width = "! android: layout-height="match-parent" tools: content="Main Activity">
<EditText
android: id d/editTextNuml" ="@+id
: layout-width="match-parent" android: android:layout-height="wrap-content"
android: hint = "Enter number!" android: inputType = " number Decimal"
android: layout marginTop="a0dp" android: layout - margin Horizontal = "20dp"/>
<EditText
android:id="@+id/ edit Text Num2"
android:layout-width="match-parent"
android:layout-height="wrap-content"
android: hint="Enter number 2" android: inputType = "number Decimal"
android: layout margintop = "20dp"
android:layout-marginHorizontal = "20dp" />

<Button
Date
android:id="@+id/ButtonAdd"
android: layout-width="" "wrap-content"
android:layout- height="wrap" "wrap_content" android:layout-below="@id/editText Num?"
android:layout-marginTop = "20dp""
android:text="Add""
android: onclick="performoperation"
android:layout-margin Horizontal = "20dp" />
<Button
android:id="@+id/ Button substract" android:layout-width="wrap-content"
android: layout - height=" Wrap-Content"
android:layout below = "@id/button Add"
android:layout-marginTop="10dp"
android:text="Substract"
android: onclick = "perform operation"
android:layout-margin Horizontal. = 20 dp" />
<Button
android:id="@+id/Button Multiply"
android:layout width="wrap-content" android:layout height = "wrap-content"
android: layout below = "@id/buttonSubstract"
android : layout... marginTop="10dp"
android:text="Multiply"
android: onclick="performsperation"
android:layout-margin Horizontal = "20dp" />

<Button
Pg. No. 13
Date
android:id="@+id/button Divide"
android:layout-width="wrap-content"
android: layout - height="wrap-content"
android:layout below="@id/button Multiply" android:layout-marginTop="10dp"
android: text = "Divide"
android: onclick = "perform Operation"
: layout margin Horizontal = "20dp" /> android:
<TextView
android:id="@+id/TextView Result"
android:layout-width="wrap-content"
android: layout. height="wrap_content"
android: layout - below = "@id/button Divide"
android:layout-marginTop = "20dp"
android:text=""
android:layout_margin Horizontal = "20dp" />
</ Relative layout>

→
JAVA Code:-
Date
public class MainActivity extends AppCompatActivity {
EditText numl, num2;
TextView result;
@Override
protected void concreate (Bundle savedInstanceState) {
super. Oncreate(savedInstanceState); setContentView(R.layout.activity-main);
num1 = findViewById(R.id.editTextNuml);.
num2 = findViewById(R.id.editText Num2); id. textView Result); = findViewById(R.id. result =
public void performOperation (view view) {
double number! Double. Parse Double(num1.getText().toString());
double number 2 - Double-Parse Double(num2.getText().toString());
double answer = 0;
Switch (view.getId()) {
Case Rid. button Add:
answer = numberl + humber2
break;
Case R.id.buttonsubstract:
answer = numberl-number 2
break;
Case R.id. button Multiply:
answer = number 1 x number2;
break;
Case Ridan button Divide:
if (number 2!=0){
answer = numberl/number 2;

}else {
Toast.makeText(this, "Cannot divide by Zero", Toast.LENGTH
-SHORT).show();
return;
break;
result. SetText("Result: "+ answer);
}
}
6.Create simple program which show the use of auto complete Text View.
And XML code:- <?xml version="1.0" encoding="utf-8"?>"
< Relative layout xmlns:android="http://schemas.android.com /apk/res/android" xmlns:tools="http://schemas.android.com/tools"
android: layout width="match-parent"
android: layout. height t="match. parent" tools: Context = "- Auto Complete Activity">
< Auto Complete TextView android: id ="@+id/autocompleteTextView. android:layout-width=" android:layout-height match-parent" "Wrap-content" android:layout-marginTop="16dp margich orizontal = "16 dp" android: hint = "Type" a country"/>
</Relative layout>


→
Java Code:
import android.os.Bundle;
import android.widget. Array Adapter;
Import android.widget. AutocompleteTextView;
import android.appcompat.app.AppCompatActivity;
public class Auto Complete Activity extends Applompat Activity {
@override
protected void oncreate (Bundle savedInstanceState) {
Super.onCreate(savedInstanceState); Set ContentView(R.layout.activity-auto-complete);
String 7 countries = "Australia" "Brazil", "Canada", "Germany, "India", "Japan", "vs"y;
Array Adapter <String> adapter = new Array Adapter <> [this, android. R.layout.simple-dropdown-item-line, countries);
AutoCompleteTextView autocompleteTextView = findViewById(R.id.auto Complete TextView);
auto CompleteTextView.setAdapter(adapter);
}
}

7.Create Sample application with login module. (check User name and password) on successful login, go to next s And on failing login, alert alert user using Toast. Also pass Username to next screen. to next screen.
Ans
XML code:
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/ap /res/android"
android:layout Width "match parent" android: layout. height="match parent"
>
<TextView)
android:id="@+id/tuname"
android:layout-width="wrap_content"
android : layout-height = "wrap-content"
android: layout margin start = "21 dp" android:layout_marginTop="49dp"
android: text = “Username”
android: textsize = "18 sp" />
<EditText
android:id="@+id/ et Username"
android:layout width="wrap_content" android: layout height = "wrap-content"
android:layout_align Baseline="@+id/tvName"
android:layout-alignBottom="@+id/tuName" android: layout align Parent End="true"
android: layout margin End = "23dp" android: ems="10"
android: inputType = "textperson Name" />

<TextView
android:id="@+id/tupass"
android:layout-width="wrap.Content" android: layout. height="wrap-content"
android:layout-align End = "tid/tuName" android: byout-below="@+id/etusername"
android:layout" marginTop="32dp" Password"
android:textsize = "18SP"/>
<EditText
cundroid:id="@+id/et Password"
android:layout-width="wrap-content" android: layout-height="wrap-content"
android: layout - allgen Baseline="@+id/tupall"
android:layout-alignBottom="@+id/tupass" android:layout - align start = "@+id/etUsername"
android: ems="10"
android: inputType = "TextPassword"/>
<Button
android:id="@+id/button"
android:layout_width="wrap_content" android: layout. height=" ="wrap-content"
android:layout-below="@+id/ expassword" android:layout center Horizontal"="true"
android:layout marginTop= ="38dp"
android:text: LOGIN”
/>

<TextView
Date
android:id="@+id/tuloginStatus"
android:layout-width="" height="wrap. content"
android: layout. android: layout. "wrap-content"
android:layout. Center Horizontal="true" android: layout. marginTop="100spe
</Relative layout>

➡️JAVA Code
package com.example.helloworld;
import androidx. appcompat.app.AppCompatActivity's ;
import android.os.Bundle Import android.view.View;
import android.widget.Button; import android.widget. EditText;
import android.widget. TextView,
import android.widget.Toast;
public class MainActivity extends AppCompatActivity & EditText etusemame, et password;
Button btn status;
TextView tvloginstatus;
@override
protected void onCreate(Bundle savedInstanceState)s super.onCreate(savedInstanceState);
Set Content View layout.activity main); et username = (EditText) findViewById(R.id. etusername);
et password = (EditText) Find view byId(R.id. et password), btnStatus = (Button) findViewbyID (R.id.Button);
tv loginstatus = (TextView) find View byId(R.id.tvinginstatus);
btn Status, seton clickListener(new View. Indicklistener Of @override
public void onclick(View v) {
Check ();
}
});

public void check(){
if (et username.getText().toString().equals("tonystark") th etpassword.getText().t etprogin status set Text ("login successful) ok
yelsef
elsact.makeText(this," login fail", Toast. LENGTH LONG). Show();
}
}
}











