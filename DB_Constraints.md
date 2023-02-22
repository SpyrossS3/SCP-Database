# Database Constraints:

Database name: scp.db

(Having two SCP tables, may be repetitive, but compartmentalizing the two large sets of data into a basic entry and then an advanced entry is better for readability and accessibility in future work with the database and when accessing information.)

(Containment Class/Esoteric Class IDs can be Null)

Library Table:

* LibraryID
  * Primary Key
  * Auto Increment
  * Int Type
  * Not Null
* SCPEntryID
  * Foreign Key
  * Int Type
* TaleID
  * Foreign Key
  * Int Type


SCPEntry Table:

* SCPEntryID
  * Primary Key
  * Auto Increment
  * Int Type
  * Not Null
* SCPID
  * Foreign Key
  * Int Type
* ClearanceID
  * Foreign Key
  * Int Type
* ContainmentID
  * Foreign Key
  * Int Type
* SuffixID
  * Foreign Key
  * Int Type
* DisruptionID
  * Foreign Key
  * Int Type
* RiskID
  * Foreign Key
  * Int Type
* EsotericID
  * Foreign Key
  * Int Type
* EntryDesc
  * Varchar Type
  * Not Null
* TagID
  * Foreign Key
  * Int Type


SCP Table:

* SCPID
  * Primary Key
  * Auto Increment
  * Int Type
  * Not Null
* SCPItem
  * Varchar Type
  * Not Null
* SeriesID
  * Foreign Key
  * Int Type
  * Not Null
* SCPName
  * Varchar Type
  * Not Null


Series Table:

* SeriesID
  * Primary Key
  * Auto Increment
  * Int Type
  * Not Null
* SeriesNum
  * Varchar Type
  * Not Null


Clearance Table:

* ClearanceID
  * Primary Key
  * Auto Increment
  * Int Type
  * Not Null
* ClearanceLvl
  * Varchar Type
  * Not Null
* ClearanceRank
  * Varchar Type
  * Not Null
* ClearanceAbbr
  * Varchar
  * Not Null


Containment Table:

* ContainmentID
  * Primary Key
  * Auto Increment
  * Int Type
  * Not Null
* ContainmentClass
  * Varchar Type
  * Not Null


Suffix Table:

* SuffixID
  * Primary Key
  * Auto Increment
  * Int Type
  * Not Null
* SuffixClass
  * Varchar Type
  * Not Null


Disruption Table:

* DisruptionID
  * Primary Key
  * Auto Increment
  * Int Type
  * Not Null
* DisruptionClass
  * Varchar Type
  * Not Null


Risk Table:

* RiskID
  * Primary Key
  * Auto Increment
  * Int Type
  * Not Null
* RiskClass
  * Varchar Type
  * Not Null


(Esoteric table data should be added as SCPs are, or I will need to add other tables such as "Object" or "Subclass".)

Esoteric Table:

* EsotericID
  * Primary Key
  * Auto Increment
  * Int Type
  * Not Null
* EsotericClass
  * Varchar Type
  * Not Null


Tag Table:

* TagID
  * Primary Key
  * Auto Increment
  * Int Type
  * Not Null
* SCPID
  * Foreign Key
  * Int Type
  * Not Null
* scp
* goi-format
* tale
* supplement
* site
* guide
* essay
* news
* resource
* joke
* poetry
* archived
* explained
* decommissioned
* 001-proposal
* collaboration
* co-authored
* safe
* euclid
* keter
* thaumiel
* apollyon
* archon
* neutralized
* pending
* esoteric-class
* adaptive
* alive
* amorphous
* autonomous
* bacteria
* fungus
* hive-mind
* hostile
* humanoid
* metamorphic
* predatory
* plant
* sapient
* species
* swarm
* tree
* virus
* animal
* amphibian
* arachnid
* arthropod
* bear
* bee
* bird
* bovine
* butterfly
* canine
* cephalopod
* cetacean
* crustacean
* deer
* dinosaur
* equine
* feline
* fish
* insect
* invertebrate
* primate
* rabbit
* reptile
* rodent
* shark
* snake
* worm
* biological
* biohazard
* cadaver
* contagion
* dental
* extremity
* genetic
* medical
* nocturnal
* ocular
* parasitic
* reanimation
* reproductive
* sexual
* skeletal
* toxic
* addictive
* antimemetic
* auditory
* cognitohazard
* compulsion
* empathic
* gustatory
* hallucination
* infohazard
* knowledge
* language
* memetic
* mimetic
* memory-affecting
* mind-affecting
* neurological
* observational
* olfactory
* predictive
* sensory
* sleep
* tactile
* telepathic
* visual
* acoustic
* chemical
* cube
* corrosive
* ectoentropic
* electrical
* electromagnetic
* entropic
* fire
* gaseous
* gravity
* immobile
* indestructible
* intangible
* light
* liquid
* magnetic
* meteorological
* microscopic
* miniature
* mobile
* portal
* paradox
* polyhedral
* radioactive
* reality-bending
* self-repairing
* self-replicating
* shadow
* spacetime
* sphere
* telekinetic
* teleportation
* temporal
* thermal
* thermodynamic
* transfiguration
* transmission
* vibration
* appliance
* artistic
* artifact
* clockwork
* clothing
* computer
* currency
* document
* electronic
* food
* inscription
* jewelry
* mechanical
* media
* musical
* online
* performance
* photographic
* robotic
* sculpture
* tool
* toy
* weapon
* vehicle
* afterlife
* airborne
* aquatic
* building
* city
* extradimensional
* extraterrestrial
* geological
* library
* location
* moon
* planet
* satellite
* structure
* subterranean
* sun
* corporate
* concept
* exchange
* foundation-made
* future
* game
* historical
* k-class-scenario
* legality
* loop
* mathematical
* military
* meta
* narrative
* probability
* religious
* ritual
* sport
* uncontained
* abnormalities
* angle-grinders
* decommissioning-dept
* ethics-committee
* fire-suppression-dept
* folklore-dept
* miscommunications
* pataphysics-dept
* procurement-liquidation-dept
* surrealistics-dept
* tactical-theology
* tau-5-samsara
* telecom-office
* unreality-dept
