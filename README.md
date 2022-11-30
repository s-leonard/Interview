# Interview


So were going to go work through a problem or more a feature that we in theory  want to build 

In this scenario we want to get a users drug schedule for a given day

So we store drug schedules

- Advil between Jan 1st 2022 to Feb 15th 2022 and I'm taking it at 07:00, 19:30
- Asprin between Jan 15th 2022 to Feb 28th 2022 and I'm taking it at 08:00, 12:30 & 15:30
- Metformin between Jan 1st 2022 to Feb 1st 2022 and I'm taking it at 12:00

Then we would have a function `getScheduleForDay()` where we pass in a given day to that function example: `Feb 9th 2022`

And it going to return the users drug schedule for the day in time order

So for example 
```
{
    "07:00"   :   "Advil",
    "08:00"   :   "Asprin",
    "12:30"   :   "Asprin",
    "15:30"   :   "Asprin",
    "19:30"   :   "Advil"
}
```

this scenario is somewhat simplified as we 50 mins

but we looking to build similar capabilities

so forgetting what we have just done and let just discuss, if this was you system and you were starting from scratch

how would you tackle this problem?
the end result is going to be similar, we need to see a persons drug schedule

- how you do model that?
- what data would you store, 
- how you store it
- how you ensure its performant 


Examples

data sctructure
```
[
  {
	"name" : "Asprin",
	"start" : "2022-01-15",
	"end" : "2022-02-28",
	"times" : ["08:00", "12:30", "15:30"]
  },
  {
	"name" : "Advil",
	"start" : "2022-01-01",
	"end" : "2022-02-15",
	"times" : ["07:00", "19:30"]
  },
  {
	"name" : "Metformin",
	"start" : "2022-01-01",
	"end" : "2022-02-01",
	"times" : ["12:00"]
  }
]
```



