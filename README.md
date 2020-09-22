<div align="center">

## Calculate the week \# of the year


</div>

### Description

Calculates what the week number is for the year, according to the current date.
 
### More Info
 
Current week # of the year.


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[DJ Hall](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/dj-hall.md)
**Level**          |Beginner
**User Rating**    |5.0 (30 globes from 6 users)
**Compatibility**  |
**Category**       |[Clocks](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/clocks__2-88.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/dj-hall-calculate-the-week-of-the-year__2-2145/archive/master.zip)





### Source Code

```
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.0 Transitional//EN">
<html>
<head>
<title>The week number of this year is....</title>
<meta name="author" content="DJ Hall">
<meta name="description" content="Find what week of the year it is.">
<script>
			//to test change Date to Date(yyyy,mm,dd) Remember for the month, Jan = 00
now = new Date()
			//Creates a date object that equals the first day of the current year.
curryearstart = new Date(now.getFullYear(),00,01)
			//valueOf() returns the number of milliseconds passed since Midnight Jan 1, 1970.
			//86400000 = Number of milliseconds in a day
dayselapsed = (now.valueOf() - curryearstart.valueOf()) / 86400000
			//calculates what day of week the year started on and adds
			//it to the number of days elapsed in the year.
weeknum = parseInt((dayselapsed + curryearstart.getDay()) / 7) + 1
document.write("Today, " + now.toString().slice(0,10) + ", is in week # " + "<span style='font-weight:bold;font-size:125%;color:firebrick'>" + weeknum + "</span> of the year " + now.getFullYear())
</script>
</head>
<body>
</body>
</html>
```

