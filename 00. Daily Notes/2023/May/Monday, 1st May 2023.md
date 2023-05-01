---
tag: dailies  
---

<< [[Invalid date|Yesterday]] | [[Invalid date|Tomorrow]] >>

> [!Quote]+ Quote of the Day  
> > It's a good thing to be satisfied with what one has.
> — <cite>The Buddha</cite>

```dataview  
Table without ID L.text As "Today's Goals"  
From #dailies  
FLATTEN file.lists As L  
WHERE meta(L.section).subpath="Action Plan" and file.name= "Invalid date"  
```

> [!tip]+ Habit Tracker  
> Sleep:: 0  
> Reading:: 0  
> Exercise:: 0  
> Meditation:: 0  
> Writing:: 0

```dataview  
TABLE WITHOUT ID  
file.link as Date,  
choice(Sleep > 7, "🟩", "🟥") as 🛌,  
choice(Exercise > 30, "🟩", "🟥") as 🏃,  
choice(Reading > 30, "🟩", "🟥") as 📚,  
choice(Meditation > 10, "🟩", "🟥") as 🧘,  
choice(Writing > 750, "🟩", "🟥") as ✍️FROM #dailiesWHERE file.day <= date(now) AND file.day >= date(now) - dur(7days)  
SORT file.day ASC  
```

> [!abstract]+ What am I grateful for?  
> - 1  
> - 2  
> - 3
> [!abstract]+ What did I consume today?  
> - 1  
> - 2  
> - 3  
  
> [!success]+ What did I create today?  
> - 1  
> - 2  
> - 3  
  
> [!example]+ Who did I talked to today?  
> - 1  
> - 2  
> - 3  
  
>[!Important]+ Highlights of the Day  
>- 1  
>- 2  
>- 3

