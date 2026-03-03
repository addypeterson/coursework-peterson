# Draft title: Distinguishing Between Marsquakes and Meteor Impacts

## Group Members (2-3): Addy Peterson

✨ Motivation: Understanding differences between marsquakes and meteor impacts allows for better understanding of new events. For example, we might be able to understand Mars' plate motions better, or estimate how big meteors are/how far away they are by how much shaking they cause. This would be super interesting, but also help to understand greater patterns on Mars to inform different space missions. 

🤔 Question and Hypothesis: What are unique frequencies of tectonic plate movements vs meteorite impacts, and how can they be distinguished from each other?

- I hypothesize that meteorite impacts will be distinct form tectonic plate movement by their higher frequencies and shorter duration. An earthquake has to penetrate through several layers of crust, which spread out the waves from epicenter to detection. Meteorites impact the surface, so shaking caused by impacts are not spread out as much by the crust.

📈 How are you going to answer/test: 
- There is a public data set called the InSightMQS Catalog which detects Marsquakes and categorizes events by low frequency and high frequency events. I could use confirmed impact events (meteorites) and compare to low frequency events of a similar magnitude (marsquakes). I would use this data to look at how long events occur for and which characteristics differ. 
- Data comes in MiniSEED format: vertical(z), north/south(n), and east/west(e), and shows frequencies/velocity/acceleration.
StationXML: latitude/longitude of the sensors, orientation, and removes noise
Catalog is basically a spreadsheet with p-waves, s-waves, distance (degrees away from the lander) and the martian equivalent of the event on the richter scale. From what I can tell these are all compatible with python and data is treated as a "stream" object- more on that later!