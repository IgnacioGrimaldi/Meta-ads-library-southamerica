# Title: South American Political Advertisers Spent at Least US$357 Million on Facebook and Instagram
A data driven story about the money spent in political content on Facebook and Instagram. Focused on presidents and campaigns in the region.

# Link
https://ignaciogrimaldi.github.io/Meta-ads-library-southamerica/

# Findings
Presidents, candidates and political parties aren't alone in the Meta's paid advertisements library. Specific information about different countries exposes that unkown or not so popular organizations also spent money promoting partisan content. For example: in Argentina one of the highest advertisers is Ratio Oficial, an entity that on its name hasn't got nothing related to politics but promote content that supports Javier Milei's "cultural battle". 

This came with a second revision of the information. Prior to that, it was possible to quantify data about each South American president and country in terms of how much money was spent, how many advertisements they ran and if they were successfull depending on the audiences they reached.

Also, the timing of the ads were analyzed. In cases like Peruvian Fuerza Popular or Ecuadorian President Daniel Noboa, more than half of their ads were released the month before elections in their countries.

# Methodology applied in the story
ABC. A = actors. B = behaviour. C = content. But that wouldn't work without a database.

# First step: search for a source, obtain the database.
With no API available, start searching for csv files here: https://www.facebook.com/ads/library/report/?source=onboarding
Obtained 12 csv files, one per southamerican country
Went to Jupyter Notebook and started a learning process in coding.

# Code work
First I clean the database and make every chart comparable with the others. So, I create a column for each csv with its country. And then convert the money values, that were expressed in local currency, into US dollars.
Then I concancatenated the 12 files in order to have one big csv, where I can run different codes with Pandas library in Jupyter Notebook and search for answers, such as: who are mentioned? how? money? ads? when?

# Mixing codes and manual work
The answer to "how much money" was difficult, because in some cases it is not the president, but the party who appears as the responsible of the ad. And also, parties may have many different VERIFIED ACCOUNTS. So, I checked manually and filtered the ones that weren't verified.
One finding: the organizations that don't seem to be political but ran political ads. POSSIBLE NEXT ANGLE: who are they? how did they support expenditures? connections with who?
In order to answer the question "when?" I downloaded more csv files from Meta. First, I analyzed which users could be representative in order to have a spent evolution among a period of time bigger than campaing months. It was check manually, among the highest advertisers.
Then I downloaded them, with help of colleagues because Meta only allows to export three files per specific individuals, per day. TEAM ALWAYS IS IMPORTANT.
When that data was obtained I just also search for the elections dates in the countries and filtered the ads that started one month before (campaign time) and compare to the total ads that every representative account supported.

# Next steps in the story with unanswered questions 
Where did the money come from? Meta informs the responsibles of the ads, but not the bank account that paid for them. Also, another possible angle may analyze the content that was promoted: which words, which images, duration and other possible quality values.
That questions may be transformed into an hypothesis and then the data-driven story transforms into an investigative story, with another methodology but with similar tools.

# Code Learning
The first days were very taugh, then I started to feel motivated. Now I think every possible story with the possibility of applying this tools in order to search for "the system" or "scale stories".

# Visualization 
Great challenge. It took me lot of time. Best advise: the easy, the best, and details at the end. By the way: I don't feel I made a good work in this area. I'm very far from being an expert. I feel in the process of learning. And in some point, in this project I learnt while making mistakes and then thinking why I was mistaken.

# Trouble
Related to visualization: I've worked with cards in Flourish, but they were very heavy. And the html file didn't work with them, so I got to screenshot them and worked in Illustrator as a png file with different layers.

# Unexplored points in database
I made focused on actual authorities. If anybody wants to go after other politicians or organizations, I´ll share my consolidated csv with southamerican entities. Feel free to use it, but also you have to know that this is uploaded by the end of June 2026. Be aware if you need to update it.
