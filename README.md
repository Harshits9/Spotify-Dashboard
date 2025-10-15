# 🎵 Spotify Top 50 World Charts Dashboard

Power BI dashboard analyzing global music trends and what's actually topping the Spotify charts.

![Dashboard Preview](https://raw.githubusercontent.com/Harshits9/Spotify-Dashboard/main/Overview.png)

## 📸 Dashboard Views

### Overview Page
![Overview](https://raw.githubusercontent.com/Harshits9/Spotify-Dashboard/main/Overview.png)

## 🎯 Why I Made This

Got tired of looking at raw CSV files trying to figure out music trends. Wanted something visual where I could click around and actually see patterns instead of scrolling through endless rows of data. Plus, I was curious - does explicit content really perform better? Are singles crushing albums? Which artists are actually dominating?

## 📊 The Dashboard

Made three pages that each tell a different part of the story:

### Overview
First thing you see - 789 songs, 342 artists, and how they're all performing. Put together some charts showing explicit vs clean content (17K explicit songs vs 11K clean), singles vs albums (562 singles destroyed the 269 albums), and monthly trends. You can see right away that October and November are when most hits drop.

### Artist View
This is where it gets interesting. Click any artist and see everything - their full catalog, when stuff released, how it performed. Found out Taylor Swift has 85 songs charting, which is insane. Travis Scott and Drake are second with 30 and 27 songs but they're not even close. Also tracked who has the most #1 hits - Lady Gaga leads with 77.

### Songs Breakdown
All the details on every track. Release dates, collaborations, popularity scores, chart positions, how long each song is. Set it up so you can filter by single vs album track because I wanted to see if the "singles perform better" thing was actually true (it is - singles average 91.86 popularity vs 88.30 for albums).

## 🔍 Stuff I Noticed

**Taylor Swift is everywhere.** 85 distinct songs in the top charts. Next closest is Travis Scott with 30. Not even a competition.

**Singles dominate.** Artists are better off dropping singles than waiting for full albums. The numbers don't lie.

**Explicit content edges out clean versions** but not by as much as I thought it would.

**Release timing matters.** October, November, July see the most charting songs. January and February are dead zones.

**"I Wanna Be Yours" leads in total popularity** followed by "Cruel Summer" and "As It Was". These tracks just won't leave the charts.

**Average song length is around 3-4 minutes.** Nothing shocking there but good to confirm.

## 💡 Questions I Can Now Answer

Before building this, I had to guess at everything. Now I can actually tell you:
- Should you drop a single or wait for the album? Single. Always.
- Best time to release? October/November or July.
- Does explicit language help? Slightly, but it's not make-or-break.
- Who's worth watching? Look at artists with multiple #1s, not one-hit wonders.
- How long should your track be? Keep it under 4 minutes.

## 🛠️ How I Built It

**Started with data** from Spotify's Top 50 World Charts. CSV file with all the chart positions, popularity scores, release info.

**Power BI Desktop** for everything - cleaned the data, built the model, made all the visuals.

**DAX for calculations** like counting unique songs and artists, averaging popularity across different groups, filtering explicit content, ranking everything.

**Visuals** - kept it simple. Bar charts for comparisons, line charts for trends over time, donut charts for splits, tables for detailed views, KPI cards at the top for quick stats.

**Design** - went with Spotify's dark theme because why not? Black background, green accents. Looks way better than boring white dashboards.

## 📈 The Data Model

Nothing crazy here. Main table with all the song data, connected to:
- Artist info for filtering
- Date table for time stuff
- Album type categories
- Explicit/clean flags

Made sure clicking on one thing filters everything else. That's the whole point of interactive dashboards.

## 🎨 What Makes It Work

**Click anything and everything updates.** Pick an artist, boom - all the charts show just their data. Select a month, same thing.

**Right-click to drill through.** Found an interesting artist? Right-click and jump to their detailed page.

**Numbers change based on what you're looking at.** Filter to 2024 only? Metrics recalculate automatically.

**Consistent look.** Used Spotify's colors throughout so it actually looks like a Spotify dashboard.

## 📁 What's in the Repo

```
├── Data/
│   └── spotify_top50_world_charts.csv
├── Reports/
│   ├── Spotify_Dashboard.pbix
│   └── screenshots/
└── README.md
```

## 🚀 Want to Try It?

```bash
git clone https://github.com/Harshits9/Spotify-Dashboard.git
```

Open the .pbix file in Power BI Desktop (it's free from Microsoft). Everything's already set up. Click around, filter stuff, see what you find.

Want to use newer data? Swap out the CSV and hit refresh.

## 💭 What I Learned

**Storytelling matters more than fancy charts.** A simple bar chart that answers a real question beats a complicated 3D thing that looks cool but tells you nothing.

**Filtering is everything.** If people can't easily explore the data themselves, your dashboard failed.

**Dark mode isn't just aesthetic.** After staring at this for hours while building it, I'm glad I went dark theme. Way easier on the eyes.

**DAX gets messy fast.** Had to rewrite some measures multiple times to get them working right. Organization is key.

**Singles really do perform better.** Didn't expect the gap to be that big but the data is clear.

## 👤 Me

**Harshit**
- GitHub: [@Harshits9](https://github.com/Harshits9)

## 🙏 Shoutout

Dataset from Spotify's charts. Power BI community helped with some DAX tricks.

---

If this helps you, star it! ⭐

**Last Updated:** October 2025
