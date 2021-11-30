# Converting ISO8601 Date format

### java.util.Date to ISO8601 date string:

```
public static String convertDateToIso8661(Date date) {
        var tz = TimeZone.getTimeZone("UTC");
        var df = new SimpleDateFormat("yyyy-MM-dd'T'HH:mm'Z'");
        df.setTimeZone(tz);
        return df.format(date);
    }
```

### java.util.Calendar to ISO8601 date string:

```
// Input
Calendar calendar = Calendar.getInstance();
calendar.set(2017, Calendar.FEBRUARY, 16, 20, 22, 28);
calendar.set(Calendar.MILLISECOND, 0);
Date date = calendar.getTime();

// Conversion
SimpleDateFormat sdf;
sdf = new SimpleDateFormat("yyyy-MM-dd'T'HH:mm:ss.SSSXXX");
sdf.setTimeZone(TimeZone.getTimeZone("CET"));
String text = sdf.format(date);

// Output
// "2017-02-16T20:22:28.000+01:00"
```

### References

* [Stackoverflow reference: #1](https://mincong.io/2017/02/16/convert-date-to-string-in-java/)
