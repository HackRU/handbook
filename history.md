# History

This is just reminiscing, but will give some context. Read if interested.

Also, a lot of this is shortened - as somebody who's seen and led this process,
I'd love to talk about it: this is the best of my undergraduate experience.

There are small quirky tales, late night idiocies, and many hilarious and beautiful
moments that are either silly or not something one would publicly upload.

So talk to your R&D directors and project leads. Because you'll realise a few things: this is a lot of fun
and they're just like you.

## Origins

R&D didn't exist before 2016. In November 2016, particularly, the name architect came to exist.
This was probably the first or second R&D thing that happened. Carlin came up with the idea and
explained it to me (Heman). It was inspired by MIT's tech team.

The name architect was probably the hardest R&D tradition that was decided in 2016. There were
many other ideas: "builders," "creators," "designers," or just "organizers" - and then we settled
on "architects." I think it's important to realise [what and architect is](architects.md#what-is-an-architect).
It's odd, since in terms of HackRU's central organization, architects are organizers.

After this, in December and January, we settled on an interview process. The familiar process
was somewhat controversial - HackRU does not interview most organizers, only R&D architects.
Carlin initially suggested that the question merely asked to generate primes.
The question that replaced it was the "contraction contraption."

## The First Wave of R&D

The first R&D email looked like this:

 > Hello there!
 > 
 > Congratulations fellow hacker!  You have passed the first challenge in becoming an Architect for HackRU!  (Actually filling out the form.)  The next step is a quick coding challenge - the contraction contraption - so we can better analyse your skills and thought process. We require that you take less than 3 days (until the end of the coming Wednesday, 1/18) to answer the questions. Please provide us with all the details that you feel are necessary to properly understand and run your code. Note that the first question asks for a runnable implementation while the second asks for a design.
 > 
 > Here are the questions:
 >   1) Write a function that takes a sentence as a string and returns a string with all the contractions instead (ie. "is not" becomes "isn't"). Convert at least [should, could, would, do, is, are, does, have] not => []n't and [should, could, would] have => []'ve. Many may occur in a sentence. Words will be delimited by single spaces and will not contain punctuation.
 >   2) Multiple contractions can be chained in some cases: there's a famous Southern "y'all'd've" (you all would have) which y'all'd'ven't (you all would have not) heard of if y'all'evn't (you all have not (I may be making this one up)) been to the South. Additionally, Scottish slang allows for "am not" to be written as "amn't," which ain't different from "ain't." Design an app to let users input sentences and get shortened (or even expanded) ones back. How would you allow them to conveniently configure your tool to handle all sorts of contractions (even their own, or their own odd chains)?
 > 
 > We hope for this to be rather conversational though in email form. Please let us know if you need any clarifications! We will send follow-up questions and hope you hear from you soon.
 > 
 > Thank you for your interest in HackRU RND and good luck.
 > 
 > Best,
 > Qasim and Heman,
 > Directors, HackRU RND.

The answers varied from tokenisers that read the input word-by-word and slowly built the new sentence by checking the words to
quick and clever hashmap implementations that grabbed words out of a hash map
and replaced with the contraction.

A hidden gem was the string "should have not" which most people made "should've not" but reversing implementations and some
hashing ones made "should haven't". Follow-ups asked about this and big-O as it was decided here that follow-ups would be nice.

The design question was a lot of fun - people discussed NLP, AI, a social media (like a stack exchange site), and various potential
mobile apps.

We were surprised that without much advertisement, we got 20 responses! Furthermore, most people were very, very talented, having
had internships, or researching AI, or just generally having bad-ass githubs. The only travesty was that we did not have any
diversity.

In the last few weeks of January we were ready to meet the architects.

## The First Meetings and Projects

The first few R&D meetings were not that great. Qasim and I did not know what we were doing.
We just kept getting late people and building their confidence without concretely defining the
more difficult projects.

We were really lucky in that Carlin took care of the main website. This became a much larger concern later on.
The projects were:
 - A slackbot (as always)
 - A day-of dashboard
 - Gavel: tweaks to the judging platform
 - QRU: a QR-code based registration system
 - A mobile app: to let QR scanning happen.
 - A photo filter: so people can update their profile pics for HackRU hype.

Another important project to mention is snackRU. Toni, the food director, thought that the QR system could, eventually,
be extended to scan the snacks and track a Hacker's consumption. This functionality somewhat existed even in Fall 2017 -
the number of serving of meals was reported to Hackers. However, the full idea was never completed. (SnackRU returns,
however, in an important sequel.) It is also notable that USACS people built a similar project but the ideas were never
communicated from HackRU to USACS or back so that the correct thing was implemented or so that the implementation was usable
at HackRU.

The photo filter was the first time we coordinated with the marketing team. This is sort of of historical importance: marketing
is the team we talk to the most. [Cong](https://github.com/CongWangStatic) finished this in a few weeks.

The day-of dashboard was a last-minute miracle. It was crashing on the day-of and just about worked, but was very nice.
It was a HackRU first and people were clamouring for it for a while. [Jan](https://github.com/jandeancatarata) did this with surprisingly little oversight,
bringing ReactJS to HackRU for the first time.

The slackbot too suffered on the day-of. However, they were the first R&D team to live on their own: they just managed and delivered
a bot with minimal intervention from the directors. [Sam](https://github.com/Azoam) led the project and was advised by [Sri](https://github.com/Sail338).

QRU and the mobile app were nice. The app was very last minute, but worked. [Steve](https://github.com/bnjw5jhyxn) wrote it in ionic and a crazy Linux set-up and learning a lot on the fly.
[Varun](https://github.com/thevarunshah) wrote an awesome backend and still maintains it! He nicely shared stats as his system was the first HackRU tech to cope with QRs.

The Gavel updates were really small and not very difficult. [Devin](https://github.com/100) finished them in 4 or 5 Git commits over the Spring break.

Another convention that was established here, accidentally, was the R&D would be responsible for registration on the day-of. This was because only we knew all the edge-cases with the phone apps and registration systems.

## The First HackRU

The eve of the first HackRU did not feel like a victory: Qasim was coding until midnight and the R&D meeting the night before had run on until 2 am with dashboard, the app, and parts of the slackbot continuously being
fixed. That night was the first for which we had the calendar too, so there was a lot of work!

Even as registration opened, R&D felt like a losing proposition: the dashboard was bugging out and hackers could barely access their QR codes.

Then, in a miraculous thirty minutes, the thirty just before hacking began, the dashboard started to work.

After this, most of R&D was smooth sailing. The mentorship bot crashed repeatedly, but one of the bugs was a certain lack of mentors. The QR codes were a revelation for the food team and the T-shirt handout at midnight,
since both ran perfectly and each hacker took very few second to process. In fact, for the first time, lines had had to be stopped so that too many hackers would not be in the food area or getting T-shirts at the same time.

The Gavel tune-up was not a tune-up: Heroku's timeout made the web scraping intractable and led to us having to fill in the database by hand. Judging was delayed by half an hour.
That said, the tune-up did let all the different prizes be supported. But we did not have enough judges to be sure that the statistics behind Gavel worked.

Overall, R&D was OK. There were improvements to be made, but that was all.

## HackRU Fall 2017

We changed the interview question to the longest lasting one:
> Hello!
> 
> Congratulations, fellow hacker: you have finished the first step of our interview process and are well on your way to being an architect! (Thanks for filling out the form.) The next step is a quick coding challenge: Heman’s tmux, a quick glimpse at your skills and thought process. We require that you take less than 3 days (until the end of the coming Sunday, 9/10) to answer the questions. Please provide us with all the details that you feel are necessary to properly understand and run your code. And as ever, please feel free to ask questions.
> 
> Tmux lets Heman code in tabs that are designated by numbers, displayed on a row from left to right. Being particular about the tabs’ ordering (on the display row), Heman has the following two commands:
> Swap: He can swap the tab he’s viewing with the leftmost tab (at which point he still sees the same code - now the leftmost tab with the same number).
> Go to tab: He can go to any tab by specifying its number. (This does not move any tabs.)
> 
> Write a program that given two tab orderings goes from the first to the second, ie:
> 
> Input:
> 0 1 2 3
> 2 3 1 0
> 
> Output: (you can omit the things in the parenthesis)
> Go to tab 3
> Swap                (State is 3 1 2 0)
> Go to tab 1
> Swap                (State is 1 3 2 0)
> Go to tab 2
> Swap                (State is 2 3 1 0)
> 
> Input should be passed as a string over 2 lines. The tab to start at is not given - always output a “Go to tab” first.
> 
> Feel free to ask questions to better understand this question. Heman does not mind demoing his tmux. Once we have your code, we will ask follow ups based on interesting aspects of your solution. Once you’re in, you will get to choose from one of our amazing projects, among which are:
> * The One App: An app for all a hacker’s/mentor’s/volunteer’s HackRU needs.
> * Sledge: a massive facelift of our judging system to allow us more control and configurability.
> * Data Display: a way to display all the data we get from HackRU. (This would most likely happen after the event, so mid to late October.)
> * Coding Samples: our awesome list of tools, other lists, and tutorials to help hackers learn at HackRU.
> * More, coming to an R&D team near you!
> 
> Hope to hear from you by Friday!
> 
> Best,
> Qasim and Heman,
> Directors, R&D.

This was a tougher interview and a few people did not complete it. That said, the standard algorithm was to take the rightmost out-of-place element and
put it in place until the desired configuration was found. Most implementations executed a linear search to locate the tab's destination, but pre-processing
this into a hashmap brought the algorithm from n^2 to the optimal n runtime.

A lot of architects were put on the back-burner since a lot of work was needed on the older projects by more experienced hands. Only 3 or 4 people were
on-boarded.

The data displaying project never happened - turns out that directors were hardy enough to look at raw JSON. This raw JSON dumper was added to the Camelot system
(in the back of OS lecture).

Gavel's statistical method proved unwieldy, so that was being re-written. [Eric](https://github.com/three) took over just after [Heman](https://github.com/hemangandhi/) made a socket-based design.
This was [Ez's](https://github.com/trestres) first project too.

Sri led the Slackbot and made it use the Twillio API to contact mentors.

The old mobile apps were merely tweaked lightly to allow for their use.

Camelot was radically altered in two ways: the frontend was moved to its own repository and short response questions and voting were added to HackRU's registration for the first time.
This was also Heman's first time being SRE for HackRU and he learned a lot about what directing all of R&D really felt like.
There were some long nights - especially one where the waitlisting system tripped on an undefined (yay, JS) and broke the site.

A tradition was added in the middle of all the development: R&D would give pre-HackRU workshops. We barely stuffed in an API one, by Sri.

Another large change was the addition of a label maker. The first successful label architecture involved Qasim's laptop running a minor node server that ran applescript (yes, a real language)
that invoked the label printer that had to be plugged in. The first successful label printing happened the Monday before HackRU at a long director meeting.

The label maker blundered on the morning of the event since the QR code backend had caching enabled. That cache generated green QR codes (in spring 2017's branding) and their greyscale
print outs could not be scanned. The cache was cleared, but only after most of registration was done - the bug was difficult to track, especially when the servers could not be restarted
as registration was happening. Qasim led a brilliant "Hacker Experience" venture where volunteers "ensured that hackers were comfortable and settling in well" while really gathering
new QR codes to print out. By dinner, everything worked out.

The Gavel re-write, now termed Sledge (the Sledgehammer to MIT's Gavel), was completed the Saturday of HackRU with Eric mostly working solo.

Sledge's debut was flawless. The only issue was that the logistics team did not realise just how functional Sledge was and panicked that they were responsible for judging.
Thankfully, this was not the case and the replacement worked very well.

## HackRU before Spring 2017

The interview process did not change, but a lot of architects finally got to join due to the easing of deadlines.

A few radical plans were in place since, essentially, Heman wanted control and Qasim wanted better mobile apps.
Additionally, other teams were waking up to R&D's potential. Also, R&D had a lot of apps and all of them wanted
to interact with the same pool of users.

The above three motives led to LCS: the API-version of Camelot. Sri joined in on this project rather quickly since
[Bryan](https://github.com/bbugyi200) (Bugyi hereafter - another Bryan is there too) took over SlackRU.
Sri, knowing the dark arts of AWS suggested that LCS use lambdas. After a bit of digging, LCS began to use lambdas.
The initial auth was not done until January 2018, but the idea was there.

Coding samples, surprisingly, had a re-birth. This project sort of floated along as something to "relegate" architects
to since it seemed to be tedious documentation-gathering. Then [Andrea](https://github.com/Andrea-Wu) suggested her vision: codecademy, but that
encompassed all of the aspects of making a web server. Sri and Heman were enthralled once they thought about Docker.
Essentially each user would be given a Docker instance and that would be their server. A socket would connect their frontend view
to the Docker. And LCS would manage the authentication! Of course, the project was handed to Andrea, and later [Kabir](https://github.com/thekabistro) joined.
A socket-based terminal emulator was completed in January, but the project was killed since tutorials were found. There is, however,
more to this tale later...

The mobile apps began work, but mostly on design since the backend was not prepared.

Sledge was undergoing beautiful re-forms, using react and perhaps the best coding culture of R&D of this era.

This was a pleasant time to be in R&D: deadlines were far and development was calm and measured.

This would change with January.

## HackHERS, WiCS, and the start of Spring 2018

WiCS did not have much of a team and runs HackHERS, the women-centric Rutgers hackathon. Though this event is a third of HackRU's size,
it is a fun and important event. It is one of three (to my knowledge) women-centric MLH hackathons and is very welcoming to beginners.
It also consistently garners excellent sponsors.

Unfortunately, most of their organizing team graduated. Hence, R&D was made to fill in the void for web development.
This was reasonable - in fact, some of the R&D vision was to unify the two hackathons in terms of code.

The lack of experience, however, made the organization very slow to respond and unaccountable for deadlines. While the hacking event
went well, this was a stressful experience for R&D's web-related projects.

LCS was ready by mid-January (with a few fixes pending). The web frontend, however, could not exist since nobody designed one.
A slew of architects chipped in. [Fan](https://github.com/fl273) helped Heman first. Then Andrea too stepped in.
The ultimate, though, was a [Connie](https://github.com/conscou)-ex-machina, where one of the alumni pushed the team and gave R&D a lot of the necessary frontend assets.

Sledge, SlackRU, LCS, and the web-frontend, were all beautifully tested and ran without a hitch at HackHERS.
Already, however, changes for HackRU were being prepared.

## HackRU Spring 2018

HackHERS ran LCS with hashing on the frontend. This was not the worst - the phone apps were not yet ready.
It, however, became quickly apparent that this was not Kosher. Instead, HTTPS was to be used.
Additionally, LCS got away without MLH login. This was added for HackRU, but in a janky way after Heman
and Sri ran out of ideas. This site was deployed over spring break, a few days late.

Designs, too were to blame, but more due to a lack of communication.

A few other changes were brewing for the backend too, however.

![I hope you see a graph...](https://g.gravizo.com/svg?digraph%20G%20{unregistered-%3Eregistered;registered-%3Erejected[style=dashed;label=%22Admin%20only%22];registered-%3Econfirmation[style=dashed;label=%22Admin%20only%22];registered-%3Ewaitlist[style=dashed;label=%22Admin%20only%22];rejected-%3Echecked_in[style=dashed;label=%22Admin%20only%22];confirmation-%3Ecoming;confirmation-%3Enot_coming;coming-%3Enot_coming;coming-%3Econfirmed[style=dashed;label=%22Admin%20only%22];not_coming-%3Ecoming;not_coming-%3Ewaitlist[style=dashed;label=%22Admin%20only%22];waitlist-%3Echecked_in[style=dashed;label=%22Admin%20only%22];confirmed-%3Echecked_in[style=dashed;label=%22Admin%20only%22]})

The registration system, following that of the Fall, was a lot more complex than HackHERS'.
This led to a lot of new logic being added to the backend system. User updates, too, were
for the first time, verified based on user privileges.

This is when some fun bugs occurred.

### That Time the Tables were Dropped

Did you know that the `$out` parameter in a Mongo aggregate truncates and then writes?
Heman didn't... Thank God MLab kept a backup...

### JS `undefined` Ruins Travel Reimbursement

Heman pulled an all-nighter to code travel reimbursement at HackNY. (If only he submitted, but T_T.) But this lead to a bug in that there was a case where
there would be an `undefined` in the JavaScript if a particular type of user applied for reimbursement. This caused the whole process to be delayed for
a week.

### Slack Rate-Limits

This killed the frontend's slack updater.

### SlackRU was not documented

Slack can't, for the life of its docs, tell you what the types of bot are. And it's hard to know which type an undocumented codebase is.
Especially when it's two types. And uses flask in an object-oriented way that's rare.

### Table Allocation Delays Judging

Yeah. The allocation algorithm crapped out, so judging was delayed as we allocated judges by hand and forced that into the table.
Additionally, there were some hacks that had to be placed close to one another, so sledge's team had to table switch by hand-querying a SQL table.

# The Moral of the Story

Document, kiddos.
