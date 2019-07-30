# ad_redesign
Redesign of Amphibian Disease Portal

# Getting AD Projects (Expeditions)
Expeditions in GEOME correspond to Projects in AD portal.  To fetch expedition data for AD portal from Geome, call:

```
# get expedition stats
https://api.geome-db.org/v1/projects/174/expeditions/stats

# get all expedition metadata
https://api.geome-db.org/v1/projects/174/expeditions?admin=false&user=false&includePrivate=false

```

# Querying Data:
```
# a simple query to get just 1 record
https://api.geome-db.org/v1/records/Diagnostics/json?limit=1&q=_select_%3AEvent%2CSample%2CDiagnostics%2Band%2B_projects_%3A174

# add in query for country = Australia
https://api.geome-db.org/v1/records/Diagnostics/json?limit=1&q=_select_%3AEvent%2CSample%2CDiagnostics%2Band%2B_projects_%3A174+and+country::"%Australia%"
```





