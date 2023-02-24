# Project: SCP Universe (Application)

This project utilizes the SCP content out there to deliver a comprehensive database of all SCP subjects throughout original works within the SCP site and will extend to content created outside of the site's works as well. Utilizing a database made with SQLite3, and GUI/script in Python, the GUI will be based on the idea given in SCP: Secret Files, where you are logged into the SCP Foundation internal network and database.

Throughout the project, content will come primarily from the [official SCP website](https://scp-wiki.wikidot.com), but also pull from games (mainly Secret Files), and possibly other fan-created works if they're worth noting. This, like all works in the SCP universe, is strictly of my own canon, and while this project's first objective above all else, is to inform, in some cases, it may be necessary to personalize alterations to better suit the project as a whole, but when any information strays from the original work on the official SCP website, you will be notified.

<br>

## Getting it done!

This will show the primary goals to hit through this project, and further below more detailed notes for the project, primarily for my own use will be noted down.

1. Create a comprehensive Excel sheet for all SCPs within the wiki
   1. Plan out the structure of the database through this Excel project
   2. Ensure the structure allows for adaptations in the future
   3. Fill out tables with SCP entries
   4. ~~Export Excel as .csv for SQL database~~ This is not feasible, as this is a large, ongoing project, so I'm going to do this little by little, adding entries in the database manually
2. Create SQLite database
3. Create base Python code to be able to access information within the database
4. Create GUI through PyQt5 and Python

<br>

### Details worth noting

* To start, I'm only doing basic entries, ~~and 001 stories will not be included at the beginning,~~ just for simplicity's sake.
  * Neither will joke SCPs, international ones, etc.
* I want to create a login dialog window upon opening the app (on first use) that allows for someone to create their profile and shows a sort of in-universe feature where "you have been granted Level 6 clearance by order of the O5 Council"
* The app will feature:
  * All SCPs
  * Joke SCPs
  * International SCPs
  * Popular media featuring SCPs
  * Information on groups, including the Foundation
  * Different canon information
  * Tales
    * The first ones put in will be ones featured on the official site
  * Any further relevant information to the SCP universe
* SCP information will follow the Anomaly Classification Guide (ACS) standard (see [here](https://https://scp-wiki.wikidot.com/anomaly-classification-system-guide))
  * This is where some deviations may exist as I will adapt SCPs where possible to this classification system
* Create the final Entry table last after **ALL** data has been compiled and entered into the database
