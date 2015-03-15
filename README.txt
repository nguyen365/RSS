RSS-- Restaurant Seating Simulator

The program takes in a file that has the list of tables and another file that has the list of reservsations and walk-ins.
The program outputs to the terminal stating when a group arrives and which table it was seated at, in the following format:
    $(Time), $(Group Size) seated at Table $(Table Number)
Groups remain at a table depending on a variable in the table settings file. Groups that reserve a table are assumed to arrive on time.

Execution format:
RSS.exe $(table settings file) $(customer file)

The table settings file should be formatted as follows:
$(Time a group spends at a table)
$(Max People at Table), $(Table can be combined with another)
..
$(Max People at Table), $(Table can be combined with another)
$(END)

The customer file should be formatted as follows:
Reserve:
$(Number of people in group), $(Time reserved)
...
$(Number of people in group), $(Time reserved)
Walk-in:
$(Number of people in group), $(Time arrived)
...
$(Number of people in group), $(Time arrived)
$(END)

The table settings file example:
60
4, Yes
4, Yes
4, Yes
4, No
6, Yes
6, Yes
8, Yes
2, No
2, No
2, Yes
16, No
10, Yes
14, No
$(END)

The customer file example:
Reserve:
4, 700
2, 700
5, 50
10, 1200
3, 1500
8, 2359
1, 0
5, 10
Walk-in:
2, 503
6, 1316
3, 1734
5, 1157
9, 552
2, 1609
4, 1525
4, 659
2, 1423

$(END)
