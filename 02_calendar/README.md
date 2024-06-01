# Project 2: Calendar

> Weight: 20% \
> Due date: June 17

When called with the keyword `new`, the native `Date` function returns
an object of type `Date`. A `Date` object has predefined methods that
allows us to know the day of the month, day of week, month, and year of
a given date.

The `getDate` method returns the day of the month according to local
time. 

```js
const today = new Date();
today.getDate(); // => 3
```

The `getDay` method returns the day of the week, where zero represents
Sunday.

```js
today.getDay(); // => 1 (i.e. Monday) 
```

The `getMonth` method returns the month as a zero-based value (where
zero indicates the first month of the year).

```js
today.getMonth(); // => 5 (i.e. June)
```

The `getFullYear` method returns the year.

```js
today.getFullYear(); // => 2024
```

You can also build a `Date` object for a date other than today. For
instance, here is how to get the day of the week for the first day of
the current month:

```js
const currentMonth = today.getMonth();
const currentYear = today.getFullYear();
const firstDay = new Date(currentYear, currentMonth);
firstDay.getDay(); // => 6 (i.e. Saturday)
```

`Date` objects can be mutated using the built-in `setDate` method.

```js
const day = new Date(2024, 5);
day.getDate(); // => 1
day.getMonth; // => 5 (i.e. June)
day.setDate(day.getDate() + 30);
day.getMonth(); // => 6 (i.e. July)
```

Using these methods, create a *dynamic calendar* (i.e., without
hard-coded values) for the current month, whichever date it currently
is. The calendar should be an HTML table where each week is a row
(`<tr>`), and each day is a cell (`<td>`). The table should contain two
header rows: the first with the full name of the month and year, the
second with weekday names (MO, TU, WE, TH, FR, SA, SU). The cell
containing the month and year should span the entire width of the
calendar (see the [colSpan property][]). Furthermore, the cells of the
current week should have a "mistyrose" background, and the cell of the
current day should have a "rosybrown" background.

[colSpan property]:
https://developer.mozilla.org/en-US/docs/Web/API/HTMLTableCellElement/colSpan

The calendar should be inserted in the `body` of the document. Beside
adding a `script` element, you cannot modify the given "index.html"
file.

Make sure to use semantic HTML (refer to the proper [documentation][]).
To manipulate the DOM, you are allowed to use only the methods covered
in class: `createElement`, `createTextNode`, `appendChild`.

[documentation]:
https://developer.mozilla.org/en-US/docs/Web/HTML/Element/table

Each task should be assigned to a separate function. Each function
should be documented using the documentation format seen in class. For
instance:

```js
// Integer, Integer -> Node
// Create a table row with a header cell containing 
// the full name of the given month and the given year.
function createMonthRow(month, year) {
    ...
}
```

Notice that a function's purpose statement should describe *what* it
does, and not *how* it does it.

## Submission

The project must be submitted in a repository using GitHub Classroom. To
create the repository, click [here][], and accept the assignment.

[here]: https://classroom.github.com/a/Cc4-16W5

## Assessment criteria

-   Requirements are met.
-   Code is readable and consistently formatted.
-   Naming is descriptive and consistant.
-   Program flow is decomposed into manageable, logical pieces.
-   Common code is unified, and not duplicated.
-   APIs are used correctly.
-   HTML is semantic.
-   Documentation is correct and clear.
