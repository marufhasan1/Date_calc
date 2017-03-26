# Date_calc
Free dll file to calculate years,months,weeks,days between two date in VB.net

## Initialize
Initialize by creating an object where you want to use.
```vb
Public my_date As New Date_calc.Date_calc
```
## Methods
* [date_diff()](#date_diff)
* [date_filter()](#date_filter)

### `date_diff()`
If you want to get differance of two date as a full string Like "2years 4months 1week 4days" you can use this method. This metho will return the full string of the difference of two string.

**Example**
```vb
Public Class Form1
    Public my_date As New Date_calc.Date_calc
    Private Sub Form1_Load(sender As Object, e As EventArgs) Handles MyBase.Load
        Label1.Text = my_date.date_diff("01/08/2014", "10/05/2017")
    End Sub
End Class
```
#### Parameters
It have 3 Parameters first 2 are mendatory and last one are optional.
> 1st 2 parameter are string formated date like "2017/01/12" or "2017-01-12".
> You can use any format using "/" or "-" Seperator "yyyy mm dd , dd mm yyyy, mm dd yyyy".
> Don't use two digit year format like "dd/mm/yy".

> 3rd Parameter are optional, you can use this parameter to get only one value (such as Year,Month,Week or Days), as integer.
#### example
```vb
  year 'To get year
  month
  week
  day
  Label1.Text = my_date.date_diff("01/08/2014", "10/05/2017", "day")
  ```
  The output will be 1013
      
      
