DateTimePicker
==============

Coolest android datetimepicker (similar to the google calendar app's one...)
Even though this calendar is not the standar calendar included by default in the SDK, lot of people we love it even more than the standard one.

Is pretty much the code here (thanks android team...):
https://android.googlesource.com/platform/frameworks/opt/datetimepicker/+/master/src/com/android/datetimepicker/date/

Quick walkthrough sample for using DatePickerDialog (more or less is the same process to use the TimePickerDialog):

Imports:

    import android.support.v4.app.FragmentActivity;
    import com.sample.datetimepicker.date.DatePickerDialog;
    import com.sample.datetimepicker.date.DatePickerDialog.OnDateSetListener;

To display it:

    DatePickerDialog datePickerDialog = DatePickerDialog.newInstance(datelistener, year, month, day, aVibrateBoolean);
    datePickerDialog.show(getSupportFragmentManager(), "datepicker");

Control the click on "done" button when you choose the date you want:

    @Override
    public void onDateSet(DatePickerDialog datePickerDialog, int year, int month, int day) {
        // whatever you're going to do with your date given by year, month and day parameters
    }

It's awesome! Isn't? :)
Happy codding!!
