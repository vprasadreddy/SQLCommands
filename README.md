SQL command to find conflicts in a given date range.

    (ISNULL(StartDate,'1/1/1753 12:00:00 AM') >= @startDate 
     AND ISNULL(StartDate,'1/1/1753 12:00:00 AM') <= @endDate)
     OR (ISNULL(EndDate,'12/31/9999 11:59:59 PM') >= @startDate 
     AND ISNULL(EndDate,'12/31/9999 11:59:59 PM') <= @endDate)
