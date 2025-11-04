<h1>Setting up a button for an android activity</h1>

STEP1:
Launch android studio and get an activity ready. See these guides on how to do this:

STEP2:
In the layout view add a button with the following mark up:

```
<Button
    android:id="@+id/buttonLogin"
    android:onClick="onClickLogin"
    />
```

Add additional styles for example width, height and color as required. The lines above will help us reference the button press in the code

STEP3:
Find the activity class that relates to your activiy with the button. In the onCreate method add a reference to your button:

<code>loginButton = (Button) findViewById(R.id.buttonLogin);</code>

Add the following function to the activiy class

```
public void onClickLogin(View view) {
//DO SOMETHING HERE
    finish();
}
```

STEP4:
Launch the app by pressing the play button at the top of the screen. Make sure you have your debug device tethered to your computer.

<hr>

TASK1:
Make an app with a single page with a button that displays a toast message when pressed
