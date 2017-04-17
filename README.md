# Final-Project

### Brief Introduction:
  
  This is the timetable APP of our team development.
  
  It is called Timetable and it is used for plan the daily schedule.



### Installation

   Xamarin Download Link:  https://www.xamarin.com/download.

    

### Usage
    axml:
    <?xml version="1.0" encoding="utf-8"?>
    <LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:orientation="vertical"
    android:layout_width="match_parent"
    android:layout_height="match_parent">
    <Button
        android:id="@+id/myButton"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="@string/hello" />
    </LinearLayout>
    
    
    
    cs:
    using Android.App;
    using Android.Widget;
    using Android.OS;

    namespace App1
    {
	[Activity(Label = "App1", MainLauncher = true, Icon = "@mipmap/icon")]
	public class MainActivity : Activity
	{
		int count = 1;

		protected override void OnCreate(Bundle savedInstanceState)
		{
			base.OnCreate(savedInstanceState);

			// Set our view from the "main" layout resource
			SetContentView(Resource.Layout.Main);

			// Get our button from the layout resource,
			// and attach an event to it
			Button button = FindViewById<Button>(Resource.Id.myButton);

			button.Click += delegate { button.Text = string.Format("{0} clicks!", count++); };
		}
	}
    }
     

                   
                   
                
           

    
     
   
    
    
