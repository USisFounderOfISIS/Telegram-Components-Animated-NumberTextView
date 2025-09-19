# Telegram Components: Animated NumberTextView
Beautiful Animated NumberTextView extracted from [Telegram source code](https://github.com/DrKLO/Telegram)

![](https://github.com/USisFounderOfISIS/Telegram-Components-Animated-NumberTextView/blob/main/Animation.gif)

Getting started
---------------
Add a copy of [NumberTextView.java](https://github.com/USisFounderOfISIS/Telegram-Components-Animated-NumberTextView/blob/main/NumberTextView.java) in your project.

Define the `NumberTextView` in XML (or you can define it in activity without using XML):

```xml
<.... NumberTextView
    android:id="@+id/numberTextView"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content" />
```

Then:

```java
final NumberTextView numberTextView = findViewById(R.id.numberTextView);
numberTextView.setTextSize(28);
numberTextView.setTextColor(Color.RED);
numberTextView.setTextAlignment(TEXT_ALIGNMENT_CENTER);
//numberTextView.setTypeface(Typeface.SANS_SERIF);
int counter = 0;
button.setOnClickListener(v -> {
            numberTextView.setNumber(counter, true, false);
            counter++;
        });
```

That's it! 
