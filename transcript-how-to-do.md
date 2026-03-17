Source: https://youtu.be/VH9uBxLJx30?si=vhVlZCgIZmWRhwmC

Introduction & Who This Talk Is For
0:00
for having me name is John Beverly as you can see here I'm assistant professor at the University of Buffalo I'm the
0:05
vice president of the national Center for ontological research formed out of UB um but it's emphasizing connecting a
0:12
lot of researchers across the world who work in ontology engineering or applied ontology which is the area I specialize
0:19
in despite being in a philosophy Department although uh maybe that
0:24
despite is not worth saying because the purpose of this talk is to explain to folks how philos phos opers provide a
0:30
lot of value in the field that I work in building ontologies and using them of
0:36
course I'll have to build up to that because I I suspect most of you so far heard me say oncology instead of
0:43
ontology um we'll remedy that as we proceed though so let me give you some background to tell you before telling
0:50
you exactly what I do so I know you've probably all heard about big data right
0:55
lots of data out there lots of it coming in there's huge amounts of data that that's uh that exists already um as of
1:03
2022 there's 147 zabt of data that's already been stored if you're like me
1:09
you thought Zeta bytes was made up and so you started doing a little digging but just to put this in perspective a 50
1:16
megabyte connection like something you probably have in your house will allow you to comfortably stream 4K videos and
1:23
at a 50 megabytes per second it would take you over 600,000 years to stream
1:28
one zetabyte of data for 147 it would take you 93 over 93 million years that
1:34
is a lot of of data um this this data so it is indeed big data right like huge
1:41
amounts it comes in at an increasingly rapid rate as the years proceed so as in
1:46
2020 um 04 zetes were being generated every day um that figure is way outdated
1:52
it's significantly higher now uh and it's only going to continue to grow um some of the sources that the data is
1:59
coming from trustworthy um academic research you know roughly speaking
2:04
trustworthy some not so trustworthy like from Twitter or X or whatnot uh and it
2:09
comes in in various standards like Json LD XML like different formats as well as
2:15
uh having conflicts that invariably emerge across data that's being stored not everybody agrees unfortunately
2:22
there's not some kind of unified understanding of how the world works and so people say things even with usted
2:28
data sources or usted documents I don't know if you've ever experienced this where you had like I don't know two
2:33
philosophers in an academic Journal arguing with one another conflicts invariably emerg as the point here and
2:38
it happens pretty regularly uh what we have a bunch of information in the world
2:44
we we're there we we want to go here we want to connect this information together in the interest of extracting
Big Data: Scale, Velocity, and the Real Problem
2:51
that that last V over there value out of it which we we still can't do for the most part now that might be surprising
2:58
to you you might you may think that John obviously we can extract a lot of value from all the data that we have we do
3:03
this all the time uh I'm I'm here to tell you that standard strategies for
3:08
extracting like knowledge or valuable information out of the data that we have stored uh in the way I've described now
3:15
is is very hacky it involves a lot of manual labor it involves individuals sitting around and looking at screens or
3:22
databases over here databases over there and trying to make connections on their own you know illustrating human
3:28
creativity but for sure a manual Endeavor that takes too long and too much effort from humans to to take to
3:35
really take advantage of especially given all the the significant amount of data we have where's nowhere near
3:41
getting to creativity as you can see now one of the reasons that the sort of big
3:47
data issue has continued to be challenging uh is it's less actually to
3:52
do with the amount of data that's coming in or how quickly it's coming in or what format it's in it has to do with the fact that it's often stored in what we
3:59
like to call information silos sure things like Management systems or databases that have content that can't
4:06
be integrated with of other information repositories using standard Computing strategies roughly speaking like if you
4:14
you put data in one database according in like I don't know in a docx file you
4:20
and somebody puts it in another database and I don't know whatever some some text
4:25
file um you have to have a way if you want to communicate or integrate that data that's stored in one file system
4:30
from another you have to have a way to integrate that now Microsoft has figured out ways to do this s but if you generalize this to data being acquired
4:37
in like I don't know the space of virology or pediatric journals or something like that and compare that
4:43
with data that's being stored from like molecular biology um where there's not like a single monolithic company that
4:49
sits on top of these these investigations or research Endeavors and says you have to you have to coordinate
4:54
in this way turns out what's going to happen is you're going to generate a lot of silos a lot of research talking in
5:00
this area and storing their information in a certain way that can't be integrated in standard Computing with standard Computing Strate strategies in
5:06
in another way so folks end up talking past each other and they often end up doing similar work nearby to one another
5:13
without realizing it this is a consequence of of siloing uh so these things manifest in various ways you most
5:22
in a lot of cases people just don't realize that certain information repositories exist and so when they're
5:27
creating their information or storing data base locally and their systems they just don't know that there's you know
5:33
similar data or nearby data elsewhere I I've been in many calls and many meetings with uh folks in government for
5:40
instance who uh where we've like gotten together a lot of groups are like a lot
5:45
of members of One agency members of another agency and we're sitting in a room and one of them somebody says at
5:51
some point this happens invariably uh if only we had data about this and then somebody else in the room goes we do
5:58
happens over and over again there's so much data out there and so many different groups working to coordinate or organize data it's very often the
Why Information Silos Kill Value
6:05
case that folks just don't realize how much is out there or what's being stored where um sometimes even like there is
6:13
awareness but there's not there's not appropriate permissions to access data so in government for instance some
6:19
information is classified and so some agencies or individuals aren't able to access information that even if they
6:25
know exists I uh you know in an open space I'm not allowed to access certain information about students I I know it's
6:32
there I just can't access it I don't have the appropriate permissions the these are reasonable reasons to have
6:37
silos I think like you certainly would want to protect some of this sort of information um more regularly I think it
6:44
is the case that uh there's simply just not the right technology in place that allows access across different databases
6:52
or different information silos and so while you can know or have access or in
6:58
a way forward even like a desire or means by which you might integrate two different data sets um you just you just
7:05
don't know how to do it in a technical sense we sort of focus in ontology engineering on addressing that um issue
7:12
which is what I'm going to be talking a lot about in the subsequent before again getting there I want to throw out this
7:18
last eye because sometimes people just don't care about integrating other repositories and so they want to create
7:24
silos and uh at least for comical effect I think that's crazy but uh so silos
7:30
when we're thinking about this in the in the context big data issues so we see that what happens is they result in data
7:36
fragmentation and often redundancy and they undermine a consolidation or integration as I said of this sort of
7:43
information which makes it seem like there's a lot more information than there is like there's a lot of duplicate
7:48
data out there because we don't know that database is talking about the same thing that this database is talking about it also creates bottlenecks that
7:55
delay information dissemination and so even though there's a r rapidly increase a rapid increase of the amount of data
8:02
coming in it can it can actually seem like there's a lot more than it is because we don't understand that a lot of the data again related to the first
8:09
volume question a lot of the data that's coming in is is already there we're just duplicating it again and again and
8:15
they're bottlenecks of of understanding what that data is so in addition the variety question I talked about how data
8:22
is housed in different formats um they're often incompatible with with formats and other information silos and
8:28
so again that variety issue comes up there's like I can't these different formats make it so that we can't
8:33
integrate also a feature or consequence of information silos as well as uh being able to leverage inconsistent standards
8:40
and undermine cross data value uh uh validation that is another consequence of information silos because again we
8:48
just don't have the Technical Resources for various reasons to to connect these standards or connect or use actually
8:54
Implement cross data validation um for these data sets and so we can't check to see if like when you say over there in
9:01
your data set that this say uh there's a a troop movement on this beach head and that data set over there maybe like an
9:09
aerial camera looking down says the troops are moving in that direction that that they are not in conflict or they
9:15
are in fact consonant with one another that happens again and again and again multimo modal data being coming in and
9:22
not being able to do cross data validation by any other means than an individual sitting there staring at a computer screen and figuring out
9:29
themselves all of this of course hinders the value obtained by integrating diverse data
9:36
so just to put a pin on that uh 2020 report by nist estimated the lack of
The True Cost of Non-Interoperability
9:42
interoperability across industrial just industrial data sets cost companies between 21 to 43 billion dollar and
9:48
McKenzie estimated midsize companies spend about 20 to 50 million annually due to these silos again these are the
9:55
issues that are causing the problems it's causing a lot of money lost so ontologies the area that I work in I
10:02
build these things I work with these things there are known solutions to information Silo challenges in the
10:07
context of Big Data not bid data but I guess that too um and what they are just
10:13
formally well-defined machine interpretable control vocabularies designed to represent entities and
10:18
logical relationships among them I'm going to spill this out quite a bit more but roughly
10:23
speaking I go I listen I look at data sets in different agencies different companies different organizations and I
10:31
regardless of how they've structured their data I figure out what they actually meant I figure out what they
10:38
really meant I think I asked hard questions to say a physicist about what
10:43
electrons really are not not just how they model them I ask hard questions to virologists about what the essence or
10:49
the nature of a virus is and I what I do is I I create a global structure future
What Ontologies Actually Are
10:55
proofing Global structure that can sit on top of different data sets and connect them all with at least some
11:00
semantic layer um so that we can use computers to reason over those data sets or extract information even though from
11:07
each of these data sets even though they're coded in different languages I give you some examples but before I get
11:13
there uh uh the if you're taking anything away from this just take these these two here these two bullets on the
11:20
bottom here ontologies as we build them here they make explicit implicit meanings buried in data sets just by
11:27
using basic principles of logic and they provide a semantic layer in doing so that connect information
11:34
silos and in doing so in pursuance of that they provide something of a lingua franka across silos that reduces
11:41
fragmentation and redundancy and they promote automated data integration and they standardize and a way to like
11:48
extract information from those data sets as well as exhibiting standard syntax and semantics and common formats and
11:54
standards while representing uh or in the represent while the representation leverage textual and logical definitions
12:01
for consistency checking to facilitate information extraction across these dispe data sets to allow for broad
12:07
integration so they hit all of these 5 vs and they have done so for a long time
12:13
and it has become well known certainly in recent years that ontologies are able
12:19
to provide the sort of benefits I'm sure you've all heard about large language models generative AI more more more
12:25
broadly um Knowledge Graph incidentally you see knowledge Network or knowledge graphs here these are knowledge graphs
12:32
are just ontologies that have been applied to data but you'll see all across here like these this top and uh
12:38
this this item at the top from the National Science Foundation is a huge Grant that was was set up for like 20
12:45
teams right now have received funding for this but what they're doing is building like about 18 different
12:51
knowledge graphs or ontologies for 18 different areas Like Water Maintenance
12:57
um like uh gosh oh the law like uh legal codes or jury or jury duty
13:02
characterizations or something like all these different data sets like 18 of them and they're going to be integrated
13:08
within a single like knowledge Network they're calling but a significant effort a significant amount of money put
13:13
forward by from the National Science Foundation to pursue this also you see here on the right the Department of
Ontologies, Knowledge Graphs, and AI
13:18
Homeland Security their artificial intelligence road map is mentioning ontologies directly and Gartner which is
13:25
on the the right at the bottom here Gartner's like future or oriented like
13:30
Tech that's going to be beneficial for generative AI they've identified knowledge graphs ontologies as the
13:36
center piece for the go for the for generative ai's wave and Improvement in the in the near- term uh as well as we
13:43
circle around here uh going clockwise to the amount of research that's been generated on knowledge representation or
13:49
knowledge graphs or ontologies from different countries over over the pr
13:54
previous years again explosion of interest in what we're doing um
14:00
but that may may just say okay John you've you've made a case see at least roughly speaking how these things work
14:06
or roughly speaking certainly a lot of people interested in them still you're a philosopher talking about this stuff and
14:13
you're talking to philosophers about this stuff which funnily enough is the first thing I thought when I sat into
14:19
talk with Barry Smith here at UB I was like yeah that all makes sense man but like why is a philosopher talking about
14:25
this why aren't Engineers handling this problem so let me EXP
14:30
little more background so 98 think about it take your mind back there 1998 the
14:37
Human Genome Project is taken off we're we're g about to crack the human genome
14:42
and find out answers and cures and like resources treatment options for all sorts of diseases perhaps we're going to
14:48
approach longevity mortality like the world is our proverbial orer uh the
14:53
geneontology was an effort that emerged nearby adjacent to the human genome
14:59
project as a way to help researchers exploring the massive data that emerged from the Human Genome Project in a
The Gene Ontology Success Story
15:05
coordinated fashion because they recognized early on that if researchers went out and kind of made up their own
15:11
terminology they would never they could never secure or ensure that they were talking about the same things while
15:16
they're modeling the human genome and so this from its early or from its Inception was aimed at providing
15:22
computational model of biological systems from the molecular to organism level across all species in the tree of
15:28
life in the interest of ensuring that folks researchers who are investigating genes
15:34
could talk to one another now when developed correctly ontologies
15:40
provide as I'm pointing to these common vocabularies or common semantics across multiple domains which is what the gene
15:46
onology was aimed to do the success of the gene ontology and it was very successful it led to a proliferation of
15:53
ontologies developed by various subject matter experts some philosophers computer scientists and logicians and I
15:59
want to highlight here when I say the success of the gene ontology it's the most successful ontology that's ever
16:04
been created it at this point there's been3 billion dollars invested in it
16:09
since 98 it is incredibly successful but in any event it was successful early on
16:15
and that that led to a proliferation of interest in development of ontologies uh none of which unfortunately at the early
16:22
on were developed in coordination with any other which resulted in a massive incompatibility of terms and relations
16:28
confusion infighting and name calling there people got on board with building ontologies but they didn't do it with a
16:34
in a coordinated fashion and that just kind of duplicated the interoperability or the information Silo is a problem
Why Ontologies Failed (and How Standards Emerged)
16:41
that at a different level of generality instead of being at the level of data it was now at the level of ontologies now
16:48
this spurred the development of a Consortium of biologists and medical professionals and philosophers who got
16:54
together and said listen we're going to come up then with a set of Standards so that we know that we're building
16:59
ontologies in a coordinated fashion one of the and you see the principles here
17:05
this is the open biological and biomedical ontology Foundry OBO now it still exists they still follow these
17:10
principles but you know at the bottom here I'm pointing out that one of the principles that they aligned to is
17:16
adopting a top level ontology starting point for all ontology development and that was created by the philosopher
17:23
Barry Smith who's a professor here at the University of Buffalo one my colleagues and bfo was adoped as that
17:29
top level architecture for the OBO Foundry and has since been adopted by many other ontology Foundry efforts such
17:35
as the industrial ontologies Foundry and also I should say across basically across all of the dod the Department of
17:41
Defense and the intelligence community and the US government so and this is a a v a picture of of this very lightweight
17:48
very minimal ontology and if you if you have any metaphysical bones in your body you're probably seeing some common
17:54
categories like continuent thing that exist in time urrent things that exist overtime you have material entities
18:01
things that have matter as Parts you have H qualities and we do mean qualities in the sense you're probably
18:06
thinking of them we also have like dispositions things that can manifest like solubility of salt but don't always
18:12
have to manifest whenever they they exist because a piece of salt stays soluble whether it hits water or not
Basic Formal Ontology (BFO) Explained
18:18
right like we allow like a very high level structure that we used as a
18:23
starting point um OBO did this we do this the industrial ontology Foundry effort does this as well well like again
18:29
a common starting point born out of philosophical and metaphysical Reflections uh started by Barry Smith
18:36
under which the gene ontology Falls uh currently over 700 projects use basic
18:42
formal ontology it is the only ISO standard I should say um for top level ontology development um so which which
18:51
is one of the reasons why it's used so widely now just to dig in just a little bit more so you can see some of the
18:56
philosophical meat here uh those boxes that you're looking at entity continuant urrent these are representing
19:03
collections of instances of things so these are classes these are classes under which instances fall so for
19:08
example the class of tables would fall under the class of objects and your dinner table would be an instance of the
19:14
former so we make this type token distinction uh also if you're looking at that you see in the upper right hand
19:20
side you'll see this ISO and what that means is arrows the class A is a Class B just means that any instance of Class A
19:27
is also an instance of class Class B which is like a you know subsetting sort of relationship now using basic formal
19:35
onology as top level architecture we we start there and we build more specific
19:40
ontologies to cover more specific on content with principles that help guide us and help us avoid mistakes but we
19:46
cover things like livers Foods tanks computers and we have principles by which we do this extension um now I
19:54
should say some of the methodological convictions again born quite a bit out of metaphysics the traditional
Realism vs Conceptualism in Data Modeling
20:01
metaphysics uh but some of the reasons why basic formal onology has been so successful and will continue to be so
20:06
successful first that we we adopt realism now I know I've I've no doubt
20:12
just raised your heckles because you're like realism what does that mean it's a vexed issue it's a vexed term in in
20:18
philosophical circles and I should say it's also a vexed term when you're outside of philosophical circles but the roughly speaking what we mean by realism
20:26
as a methodological conviction here is that are the ontology is designed and its extensions are designed to represent
20:32
the world rather than just Concepts about it now there are ontologies out there that follow what we call
20:38
conceptualism where you're attempting to like model the way we conceive the world
20:43
to be rather than the way the world is and we we reject that we want an external Arbiter we want to make sure
20:49
that we are focused on trying to model the real world rather than just the way
20:54
we think the world is and one of the reasons is just a practical reason is right here if we attempt to model the
21:02
words we use and go to the world it's unlikely we'll end up in the same place but if we attempt to go from the world
21:07
to the words we use it's much more likely we remain coordinated and I see this again and again if I usually I'll
21:13
do some kind of active learning at this state but I I I won't I won't belabor that here but the idea would be I would
21:19
ask the group I would say give me each of you individually give me your best definition for
21:26
car and I suspect you know we'd get quite a few different definitions for
21:31
car and those would be your conceptualizations of what car is and then we could argue we could we could sit here and argue about which
21:37
definition was right and I think that's just the wrong way to approach this sort of modeling what we should do is find
21:43
what's core across the definitions where maybe what's core what what an actual car is
21:49
like the nature of it the essence of car right and then we start from there to
21:55
extract the way you think or conceptualize the car so inste again we
22:00
try to focus on the word world and then from there we can extract the words rather than focus on the words and go to
22:07
the world and uh this is important for us to point out because it is very often the case very very very often the case
22:14
we're dealing with people who are not philosophers they are modeling things out there in the world based on whatever
22:21
or how whatever strategy they were taught um at you know at at Mother's knee they will invariably model the way
22:28
they conceive things rather than aiming at the world and it is almost in every case different from the way other people
Roles, Dispositions, and Why They Matter
22:35
model world or the words so we again try to get ahead of that by emphasizing realism we also want to point or I want
22:43
to point out here that adequa ism is another methodological conviction we have uh bfo itself is non-reductive uh
22:50
we take classes and relations that are motivated by the research communities we deal with and we don't try to paraphrase
22:55
them away to illustrate this is a picture of here he's an instance of the class agent which is a subass of objects
23:04
which is a subclass of material entity and if I were to follow this up an agent is just an object that can engage in
23:11
intentional activity and an object is is a material entity that has like boundaries such that if you were to move
23:17
some internal part of the object other parts of the object would have to move as well and a material entity is just an
23:24
uh it's an entity that has matter as parts now Barry's an instance of agent he's certainly an intentional one uh and
23:30
he's also though a Sunni distinguished professor of philosophy and the Julian Park chair now I suspect uh it's it's
23:38
not at all contentious that you would want to include Barry in your ontology of the world right like even perhaps the
23:44
classes agent object material entity but it may it may shock you a little bit to know that we include as first class
23:51
entities things like roles and indeed Professor role which Sunni distinguished professor of philosophy Julian par chair
23:58
this is instance of a professor role which itself is a role which itself is a realizable entity where a role is a sort
24:05
of uh a property of you that may give you powers or may be able allow you to
24:10
manifest certain certain behaviors in certain context but it's such that if you were to lose it or gain it nothing
24:16
materially about you has changed so if you recall earlier i' i' said there was a class called dispositions where like
24:23
solubility of salt if you think about that for a second dispositions these are things such that if you were to gain or
24:30
lose them something materially about you is changed if salt is no longer soluble something about its lattice structure is
24:36
change and those are contrasted with rolls which is a sibling sibling class uh rolls are they they're missing that
24:43
kind of material basis requirement if Barry gets fired for whatever reason tomorrow nothing material about him
24:50
would change there's but nevertheless they both roles and dispositions allow you to realize different things in one
24:56
case solubility and the other case uh I guess getting grant money or holding a lot of sway at UB that's much more
25:04
likely so uh we also represent as first class entities the relationship between the instances in this case Barry and his
25:12
Sunni Professor role we say that Barry is the bearer of this role and we represent all of that explicitly in our
25:19
ontologies and this is worth pointing out because what we're trying to do is create this again semantic layer that
Making Implicit Meaning Explicit for Machines
25:25
sits the top on or top database bases and we're making explicit the implicit
25:31
semantics in those databases and so so that computers can use those resources
25:36
to extract information or connect or integrate the data in the respective databases now to do that we have to be
25:42
very very explicit because drum roll please computers are dumb and they do exactly what you tell them and no more
25:49
or no less and so if we want if we want computers to reason through or to
25:54
integrate data that's connected in the way I've just described here Barry Smith bear of a Sunni Professor role we have
26:01
to literally specify that because the machines are not going to infer that
26:07
information lastly here I'll say fism is another one of our methodological convictions we while we take our lead
26:13
from scientific research as it stands we understand that might change and if you're familiar with David Armstrong we
26:19
kind of take both adequa ISM and and well not not exactly adequa ISM but some of adequa ism adequa ISM and fism
26:27
straight from him so we are taking our lead as to the nature of the world from
26:32
researchers who are investigating it this is not to say that we don't we always agree with them we do not I'll show you some examples of where we come
26:40
come apart but we definitely take that as a default starting point they may be wrong and we're open to changing as a
26:46
consequence whether it be even at the tippy top with bfos as a top level architecture or Downstream when we
26:51
extend down to more specific domains uh so again bfo high level
26:57
structure rure extend from it into more specific content um we do that in by
27:03
providing in this downward population strategy where we start with something in bfo whenever we're trying to model
27:09
something on the ground like a table or a chair uh and we we always try to find
Hub-and-Spoke Ontology Architecture
27:15
where it might fall in the subclass hierarchy of bfo and then we start introducing introducing subclasses and
27:21
subclasses and subclasses and we we find our way to the ground um in doing this we find that it provides guard rails for
27:27
promo alignment across ontologies it helps ensure that they have kind of somewhat common semantics um and what we
27:34
talk about it in terms of having like spokes that share a common semantics um with in so far as they have a common Hub
27:41
um still okay I I pointed out some of the methodological principles I have gestured at some of the like
27:47
metaphysical background they're stemming from in the philosophical literature um and I pointed of course to Barry who's
27:54
one of the Pioneers in this field all philosophical in nature now you might be asking fine why are you here today of
28:01
why more philosophers okay first and foremost I got to highlight we come up
28:07
with definitions regularly we're trying to Define things we're trying to Define things that are common we're trying to find the essence of the nature of the do
28:13
domain or domain level content things on the ground like livers and and Rubik's cubes and viruses and whatnot and coming
28:20
up with good definitions is very challenging even I mean you know it's challenging youve I'm sure you've done it before but it's even more challenging
28:26
to folks who aren't trained in it uh let me give you an example this is just a a high a relationship of some of
28:33
the um Rel or ontologies that or one of the ontologies directly that sits under
28:38
basic formal ontology called the Infectious Disease ontology and then some ontologies that extend down from it
28:43
like uh the brucelosis ontology the influenza ontology or the Corona virus infectious disease ontology now I will
28:51
hide this is from my own work where I've you I'll show you where I've used my own philosophical background to like make
28:56
progress in the construction definitions and and direct research uh researchers who are much more knowledgeable about
Case Study: Are Viruses Organisms?
29:03
the content I'll be discussing um in uh you know a more precise Direction than
29:08
where they'd been headed before so some biologists in our our community who are trying to model things like
29:13
viruses um they would count uh they they would use a definition like the sort of the sort that I've I've got here before
29:20
you an organism they'd say an organism is an object okay object is from basic form onology as you recall um and it's a
29:27
living individual system such as an animal plant bacteria or virus that's capable of replicating or reproducing a
29:33
growth and maintenance in the right environment and it's an or and they also add that as part of the definition an organism may be unicellular are made up
29:40
like humans of many billions of cells divided into specialized tissues in organs which implies I don't know if
29:46
you've noticed that viruses are cellular entities which is not true at all viruses do not have cells it's one of
29:53
the the character or defining characteristics of them they're not composed of cells like we are this now
30:01
other biologists in our community who had thought a little bit more about this uh when it when this issue was raised
30:07
thought of replacing organisms with a Class A Class that said organism or virus or viroid just to draw the
30:13
distinction um but this this disjunctive class that they've introduced or we
30:18
attempting to introduce as a way around the problems that I just pointed out lumps in viruses and viroids in with
30:24
paradigmatic living things like organisms right so why am I bringing this up well it leads to naturally to
30:32
fascinating questions like are viruses or viroids Alive what does life mean
30:37
what separates living from non-living things and I'll say none of these questions as interesting as they are
30:44
needed answering for the purposes of modeling viruses with ontologies it's just not like I agree as a philosopher I
30:52
am fascinated by these questions there's a lot of research on these questions in virology journals and biology journals
30:58
more broadly they talk about this they argue with one another and there's not a consensus around it now what I try to do
31:05
when I'm modeling viruses is be neutral because I'm I'm not trying to tell the virologists what to do I'm not trying to
31:10
be prescriptive about the way they use language I think they'll figure it out at some point they'll have some criteria for distinguishing what's v what's alive
31:17
and what's not much like they did with PL or their physicist did with Plato or Pluto when they excluded it from the
31:22
list of planets I suspect somebody will will reach a consensus here so I don't want to prejudge
31:28
um and I'm not it's not really important for most modeling tasks of viruses to answer such a question but I tell you if
31:34
you go to a meeting with virologist or biologist and you start talking about viruses invariably somebody's going to
31:42
ask you whether they are alive and if you are like me you will just say I don't need to answer that question but
Why Philosophical Questions Can Break Ontologies
31:48
why is that important here well I think to me this highlights some of the value of philosophy some of the value that I
31:54
bring from philosophy so philosophical questions we're undated with them and they're often fascinating so much that
32:00
they capture the minds not just of us but of subject matter experts researchers are asking whether viruses
32:06
are alive because it's a very interesting question and it's hard to break away from but we we're steeped in
32:12
these fascinating questions we know them when we see them we get trapped in them too but we're much more familiar with
32:18
them and because of that familiarity I think we have a firmer grip than the subject matter experts on when certain
32:25
fascinating qu philosophical questions are not relevant to a given task and I've seen this again and again both with me and my students like we know where
32:33
where the interesting questions are and we we're familiar with them and we also know when the fascinating questions need
32:38
to need to be dug into and when they can be put aside for later now check this out this is a lanan
32:45
hierarchy this is a screenshot from an ontology by the way um just a hierarchy you see all like you carry out all the
32:52
way down to brucelosis human patient wow it's really gross I I I hate this it's
32:58
nasty uh it was developed by a physician with very good intentions though he was really trying his best to to create a
33:04
model an ontologically precise model to to again extract that implicit
33:11
information across databases and making it explicit so we can like reason or connect these things right now this is a
33:18
portion of the Ido Brew hierarchy this is that that infectious disease ontology for brucelosis and the classes the only
33:24
classes in that ontology that were relevant to the task of that the researcher was investigating um were
Fixing Bad Biological Hierarchies
33:30
just those below h i that's all they needed but they built all of this other nonsense on top of it because well I
33:38
mean they were trying their best really I don't want to throw them under the bus too much now you would see this again in V virus ontologies you see this again
33:46
all over biology now I built at the height of the pandemic I was building ontologies for viruses we were we're
33:52
focus on Corona viruses of course we're trying to create identify or use the Machinery that we we leverage um in our
33:59
practice to to identify treatment options we were successful in a couple of cases but to even get there I needed
34:04
to have a kind of robust model of viruses and I did not want to do
34:09
anything like this this was messy and so what I did was I I read a lot of
34:16
virology work I read a lot of research and I've found um and that there is a a
34:22
Sevenfold PA a Sevenfold strategy for for characterizing viruses that's in
34:27
most virology textbooks called the Baltimore classification now you'll usually find it in footnotes you usually
34:33
find it in passing um but basically it's a way of structuring vir all the viruses that we know of into um in so far as how
34:42
they or what what steps they need to go through to get to messenger RNA which is
34:47
that that little highlighted box in the middle of that that diagram there all viruses have to go through that step if
34:53
they're going to to replicate but different viruses have different you know genetic structure and so different
34:59
viruses have to go through different steps maybe through RNA to DNA to positive negative DNA but ultimately uh
35:06
to that messenger RNA so it turns out that because of this this kind of bottlenecking you can represent all the
Baltimore Classification as a Modeling Breakthrough
35:12
viruses there are according this Sevenfold scheme now this is a lot cleaner than a lan hierarchy I'm sure you agree and when I pointed this out to
35:20
V virologists who were building virus ontologies in our field they in every
35:25
case almost they said wow I really wish sh thought of that look I was not a
35:30
specialist I'm not a specialist in V virology uh and philosophers more generally are not specialist in the
35:36
scientific disciplines we're we're working in when we're working as on Plat onist because of that we're not Theory
35:41
Laden we're not practice Laden we're not we're not uh you know strategy Laden with whatever the scientific domain uh
35:48
teaches its students at the same time we are trained to frame problems in multiple ways and identify subtle
35:54
conceptual distinctions and then justify our positions to the extent possible I was ready with arguments if anybody had
36:00
anything to say about the use of Baltimore classification fortunately they were kind of on board with it initially because it's so much cleaner
36:06
but in my experience though these characteristics resulted in kind of a an openness to solutions to ontology
36:12
modeling that hadn't been previously considered such as the Baltimore classification I I mean I'm not joking
36:18
many researchers in our community have been trying to build VAR virus ontologies and had been building virus ontologies before but not a one of them
36:25
had suggested a cleaner hierarchy like the one I proposed here it's born straight out of the textbooks from their
36:31
own field let me throw another one at a verion you guys know what a virion is
36:38
it's a virus in its assembled State consisting of genomic material surrounded by coding molecules you can
36:43
think of it as like the minimal the minimal virus like a minimal it's like a one single virus if you had to you would
What Is a Virion? (And Why No One Agrees)
36:50
it's the thing you would count if you were counting a virus in fact it's the thing that that's counted in titration
36:55
when they're trying to determine how much virus you need to cause an symptoms or something so but if you ask five life
37:01
science researchers what this term means you will no doubt get at least seven incompatible answers and uh options for
37:09
understanding these just just to illustrate are things like a verion is to a virus as a viruses du a verion uh
37:16
that's uh all of these by the way I found evidence for and you can read more about in a paper I published in plus one
37:21
but I found evidence for in virology literature in medical literature um there's a paper that says Vons are just
37:28
viruses there's also a paper that or several papers that think of verons uh
37:34
like uh to as to viruses as human gametes are to humans or uh but also
37:39
researchers saying that verons are to viruses as human students are to humans so something like a roll you take on or
37:44
the virus takes on or similarly virion is to a virus as a human child is to a human like a earlier on in the
37:51
development stage of a virus it is a virion now in some of in fact I found in a textbook as a matter of fact fact um
37:59
one researcher at least talking in two different ways uh I think what happened is they defined V virion in one way and
38:05
then several paragraphs later they realized that that wasn't going to work for what they were doing and so they
38:10
introduced a second definition for it and they were in conflict and I guess they never edited it but um what really
38:18
chew on this I'm not going to tell you which way I went you can read the paper just chew on it but uh but what I want
38:23
to point out here is that I was looking at this research I didn't want to exactly come down and take a firm stand
38:29
but I did use knowledge of phase and substance sortal external internal properties and stuff to to make the case
38:35
clear to researchers in the community who were building ontologies around viruses that there were there were kind
38:41
of subtle issues they needed to address or think through if they're going to start characterizing verons in one one
38:46
or more ways and also I was I was using some of this to identify inconsistencies in the way they were talking which
38:52
helped clear up some verbal disputes that were going on it made s really a range of options for interpreting the
38:58
varied incompatible ways that researchers use virion uh all in the interest of identifying some
39:03
ontologically sound definitions that helps accommodate how most researchers use the term again I leverag a lot of
Modeling Pathogenic Dispositions
39:11
philosophy to to make these cases now one other viruses are often in the
39:17
literature you see they're described as being obligate pathogens a pathogen of course is not used consistently in life
39:23
science research um and unifying that ambiguity seem to require like a deep understanding of pathogens and my As I
39:30
understood it as index to species or to stages in the development cycle of a species now this this the literature on
39:37
pathogens is is all over the place researchers talk in many different ways they talk about pathogens as like
39:43
specific material or types of material things they talk about pathogens in terms of what they can do they talk
39:49
about pathogens as like measurements of things and they often do this without being very clear about what they mean
39:54
and so that generates a lot of confusion and researchers talking past each other I think there's kind of like a core way
40:00
to understand viruses in so far as they're pathogenic and that that goes back to what I was describing earlier
40:06
about their dispositions or the dispositions to do various things uh uh
40:11
pathogenic things and so I had propos this definition which is quite complicated but uh in the best of
40:18
possible ways so I I think of a pathogen as something that has a pathogenic disposition which is just a disposition
40:24
born by some material entity to localize or produce toxins that can be transmitted to an
40:31
organism uh either of which may form a disorder in that organism or immunocompetent members of the organism
40:36
species this is quite complicated right but it was necessary I thought I still do necessary to have this kind of
40:42
breadth to capture the way that folks were in their the research communities were talking about dispositions while
40:49
respecting what seemed to be going on as a matter of fact in the world namely like I have various cases as you can see
40:56
here like cot is supporting some of this researchers talk about botulinum as a pathogen but
41:02
botulinum like for instance doesn't actually like localizing you as to
41:07
exhibit its pathogenic properties what happens is it kind of it might be like
41:13
sitting around or like moving through your system while producing toxins that generate disorder in you it's not the
41:19
same as as uh like SARS Co 2 which localizes on you and starts infecting
41:24
your cells with various like nasty nasty replication cycle features or or sta
41:30
lakus orus which is an opportunistic pathogen that also localizes in you in the right context so again why am I
41:37
highlighting this so philosophers as I said as probably clear from now are often trained in conceptual analysis
41:43
formal logic and we extract information from dense philosophical texts we train our students to do this we do this
41:48
ourselves this training not only AIDS philosophers when identifying subtle distinctions and area or research areas
41:54
outside their interest but also AIDS them with coming up with you using common applications employed for
41:59
ontology development like I spent I I thought very deeply about the way that researchers are using pathogen and I
42:06
could see a common structure across the way that we're using it now it's not exactly pretty but it is informed by
42:13
what's going on out in the world and it was good enough to get a lot of folks on board to say you know this is this is actually as vexed as our use of pathogen
42:20
is is actually not that bad it really covers a lot of the cases now I'll just
42:26
summarize here and then I want to talk about one other thing um but summaries so far philosophers tend to have a
Why Philosophers Excel at Ontology Engineering
42:31
firmer grip on when certain fascinating questions are relevant or not and they tend to be open I find in in my
42:38
experience to more possible ontology modeling Solutions than other researchers in their specific fields and
42:43
we're trained to identify definitions that accommodate disperate use cases um using some of the metaphysical training
42:49
that we get or logical training that we get uh as well as the conceptual analysis training that we get and the
42:55
ability to persuade others to to coming on our side now I said one other topic
43:00
and then then we can discuss it at your leisure but I do want to highlight though I mentioned that there are a lot
43:07
of people getting on board with the ontology engineering a lot of people getting on board with unifying data sets or connecting information and I will
43:14
also add a lot of people are getting on board with philosophers doing this work so here this is just from yeah this is
43:20
just from LinkedIn uh ontology all over the place people are looking for ontologist to hire to do exactly this
43:26
sort of thing thing that I've been describing in this talk uh note too though that in many of the required skills or basic qualifications you're
43:33
going to see philosophy pop up they they know philosophers are good at this I will I will share this anecdote with you
43:39
as well I I used to work at John's Hopkins in the Applied Physics lab before becoming a Prof Professor here
43:45
and I worked on a team with researchers like machine learning Specialists folks doing like standard NLP but also folks
43:53
working in chemistry and virology and we worked as a unified team using ontological solutions to help do things
43:59
I can't actually talk about but I will say at various points um researchers
44:05
well-meaning researchers were get into disputes that bordered on philosophical and they would call the
44:11
philosophers and that was a common thing that you would see in the slack channels or I would get an email said we need to
44:17
call the philosopher in and they weren't joking they weren't saying it factiously they would literally say in meetings called a philosopher I don't know how to
44:23
handle this question it's too much they got an they got a feel for the depth of the sort of questions they needed to
44:29
address and they hired philosophers to handle them philosophers who had like an ontology engineering background of
44:35
course but nevertheless philos philosophy was front and center why they were we were there um now so I one thing
The Job Market for Ontologists (Yes, It’s Real)
44:42
you can take away from that is that if your you know your parents ever give you grief for being a philosopher or
44:48
something they say what are you going to do go work in a philosophy Factory yeah maybe like that that's the upshot maybe
44:53
you will uh also I'll point you can point this out he like six figure entry level jobs and if you don't believe me
45:00
just ask our community um this is an incomplete list but these are philosophers just from our just from UB
45:07
that are working in philosophy some of them work here so Regina there is hired recently as a an ontologist we we
45:13
schooled together at Northwestern she followed me over here which I'm happy for but a lot of these are graduate students that born out or came out of UB
45:20
again as I said there's are incomplete list there are quite a few um and they are making quite a bit of money more
45:25
than I am um but and we are all over working in whether it's in government organizations whether in Banks um
45:32
whether in like think tanks um whether like over here at La Hoya Institute we have like research Labs also at
45:38
University of Buffalo um our researchers are everywhere and uh there's I can't I
45:44
can't tell you enough like we H just just Barry and I get requests for talent
45:50
it every other day and we do not have enough people to send that is just the
45:56
state the game I any graduate student here who wants a job has one uh our
46:02
undergrads have jobs they don't they they probably shouldn't but they do like the field is on fire and we are a
46:10
centerpiece of the flame right like people look here for talent to do this sort of work in various sectors and as
46:16
I've said as I'm saying like we we just don't have enough people to send out um so we're always kind of looking for help
46:23
and always and because of that because of the need and uh my fear uh about the
46:28
fate of the field um has led me to to do what I'm about to describe but let me say I I say I say I'm I have a bit of
46:35
fear about the field so ontology engineering is it's taken off it's it's on everybody's lips knowledge
46:41
representation Knowledge Graph on everybody's lips this is not the first time this has happened it's at least the
46:46
third time in the history of artificial intelligence in previous eras when ontology engineering has been popular
46:53
what has happened is there wasn't enough talent to feel the labor Gap and uh
46:59
researcher or like hiring managers at different universities or different Industries or different corporations
47:04
they would look around their field and they would say well who can do this work well well Jake over there in accounting he's he's heard about taxonomies before
How to Get Into Ontology Engineering
47:11
so put him in charge of this huge project and then when it failed because Jake had no idea what he was doing um
47:17
they would just put Jake back in accounting and they would blame ontologies it's easier to do that than
47:23
to say well maybe we made a mistake and so I am I am worried I'm bit fearful
47:29
that um this will continue happening if we don't Supply or like meet market demand for the ontologist and so I'm
47:34
very keen on making sure that we have folks who are well trained and trained well enough to do the sort of work that
47:41
we do and so I spent a lot of time training um both like as part of you being outside of it so here I'm just
47:47
going to highlight and I and I'm walking through this not as a sales pitch I'm not trying to take anybody from any
47:53
University I think where you are is good and you should stay there and learn your philosophical chops but if you are interested in joining or learning more
47:59
about this everything I'm about to talk about is open to the public remote recorded and the minutes through online
48:05
here and you're welcome to join slack so but here just uh ontology and intelligence analysis we work with a lot
48:12
of government folks uh and so I have I'm teaching a course about how you can apply ontology engineering to
48:17
intelligence an analysis there's a picture of the the GitHub REO and a link to it as well again all open source all
48:24
the lectures are there all the videos are on YouTube you're welcome to check them out uh also Logic for ontologist
48:29
where I get into the real technical weeds I'm a logician by training so I really love this course a lot but and if
48:35
you want to see more about that you can go look at the YouTube channels and also perhaps join the slack uh as well as
48:41
these standing uh meetings that we have and we've had for several years that cover various topics at certain levels
48:47
of sophistication in our community ontology 101 of course is the intro happens every Wednesday 11 to 12 also
48:53
open public remote meetings are recorded and all online uh as well as some of the more sophisticated uh or a little more
49:00
sophisticated ontological meetings like the Common Core ontologies one of our bigger extensions of basic formal
49:06
ontology a group of people are focused on just applying that in various circumstances and then lastly there that
GitHub as a Portfolio (What Employers Look For)
49:12
semantic mapping U uh meeting that that's that's kind of in line with the logic frontlist work it's it's really
49:19
technical stuff again I love it I'm smiling as I'm talking about it I can't help it because I love formal stuff but
49:25
anyway you can find more information about all of that on this this web page here incor on you're I'm highlighting
49:30
here the incor on 101 working group but you can see over the left we have quite a few others and a misspelling of
49:36
graduate applied ontology Society for some reason which I'm going to fix after this but uh with that I will stop and uh
49:43
let's chat
49:58
I have I have a question I don't I couldn't figure out how to raise my hand find it
50:03
um so one of my good buddies uh he's he's an ontologist he works he's been doing it for I forget three or four
50:10
years and I've when I go and visit him I ask him what he does and he sits there and he shows me what he does
50:16
and a lot of it seems like he's exploring ontologies like he's doing
50:22
queries right yeah and um I just I guess my question
50:29
was is that what you do most of the time just explore ontologies and I guess like get rid of redundancies or I don't know
50:36
even if you get rid of redundancies but like do you spend your time sending out queries and trying to find where there
50:42
might be I don't know holes in the ontology things missing and then build is like querying seems to be a big part
50:49
of like being an ontologist for some people for sure okay so so they're different like areas of emphasis right
50:56
like some people do more or less what I've described here we're like talking with subject matter experts and like
51:02
really trying to think carefully about this structures they have in mind and like there's there's so much loow
51:07
hanging fruit out there that still needs to be modeled um that that that's going to be a an opportunity for a while right
51:14
as we Explore More and More the world um but then there's also the the information extraction side and like
51:20
okay people do both like I do both um but you you can you can like use various
51:26
like query languages to like extract information from databases um with or without ontologies you can you can like
51:33
provide to help like structures to help you gain information or extract certain types of inferred information from
51:39
ontologies and I mean I like doing that because it's a it's a way to explore
51:44
like that implicit information that's being embedded in like there's once you build a structure well enough you you
51:52
you have like such a rich a rich environment to like identify h es or
51:57
identify like Newar areas and I'm I'm honestly in this I'm in this game
52:02
because I want to be immortal and I have no idea how to like gear research that
52:07
way but I assume I'm I'm hoping that if we like integrate all the data and start
Querying, Logic, and the Technical Side
52:12
querying it then I will find such a path and I'm trying desperately to do that before I die so but like column A and
52:21
column B they're also folks who kind of just do the formic side of what we do so
52:26
there's like a there's a what we call it's called description logic it's it's weaker than first order logic it only
52:32
has binary relations for instance and it kind of underwrites all the representations that we do which raises
52:39
raises challenging puzzles when you're trying to represent like I don't know John having a part or hand part at one
52:45
time and not having a hand part at another if you're familiar with David Lewis and like disputes over the ways
52:52
you might like like model like time like those same questions come up in these
52:59
like engineering discussions which is fascinating to be but so there's some researcher that Focus largely on the the
53:04
formal side like trying to identify more or less expressive Logics that we can
53:10
use while and and the the barrier that we meet is like we don't want to make it so expressive that it's undecidable
53:16
which is why we don't just use first order logic because first order logic itself you you can't always be sure if
53:21
you said something false that it's you're not looking at a loop like and so so we're there's like Balancing Act and
53:27
it's kind of underdeveloped honestly so yeah I work in that area if anybody else wants to join me feel free but those are
53:33
just three off the top of my head like different different areas you might emphasize when you it's I guess kind of
53:40
a followup real quick knowing query languages and just being able to run queries it it is is it
53:47
it's an essential skill for an ontologist no I think so okay I think so I I also I teach a lot of it um okay and
53:56
uh but honestly like it used to be it used to be a bigger barrier to entry because mostly familiar at all with like
54:03
like queering language is a sequel which is really widely used for for like
54:08
relational database structures which don't have the same structure that we use and there's so much support
54:14
textbooks and courses for SE our our community has Sparkle which is Sparkle
54:21
and there's you probably know there's not that much support not a lot of textbooks on it not a lot and so it used to be significant barrier but now with
54:28
generative AI uh I I actually teach my students I'm like I just need to teach you the right prompt so you can get
54:35
it'll write the query for you just use that okay much less of a barrier okay okay yeah that's helpful
54:42
and I would encourage you like it's not perfect you know you still need to understand it like bug but
54:50
like at least you don't have to type all that stuff out over and over again yeah they get they get pretty long yeah
54:55
really saves a lot of of the hassle so okay okay yeah that that's that's helpful thanks
55:01
yeah yes well yeah know I guess I had a follow up on Josh's question which was
55:06
um one thing that ran through my mind in your talk was just um a question about whether being a data ontologist Will
55:14
Survive like the the large language model Revolution like is this the kind of work that is protected from being
Will AI Replace Ontologists?
55:21
replaced like part of your response to the previous question seems to indicate there's a large part of the job the coding part that you really don't right
55:28
you know need a a human you just need a prompt engineer yeah I that's a great question I think the answer if
55:35
anything uh generative AI just kind of like highlighted how valuable and hard
55:40
what we do is and so the answer to your question is there's going to be space for us so like generative AI can do
55:46
awesome things it's really cool like I I'm very impressed but it's also like of
55:51
this it's it's just the most sophisticated attempt at addressing like
55:56
showing the value or showing the truth of the scalability hypothesis like it was basically throw enough data with the
56:03
right kind of reinforcement you're going to get like something like generalized AI or something you can answer it all sorts of question it'll give you the
56:09
right answer and you can be confident them but like this this this thing was so
56:14
expensive so expensive so intense so much data all poured into this best case
56:20
scenario and it still sucks and what is it missing well I mean it's missing logic basically logic it's missing like
56:27
create like like actual creativity like not the sort of creativity that can write you know decent enough High School
56:34
poems but like the you can tell when it writes a good poem or when when you see a generative AI poem when you see Keats
56:40
right like there's a difference now what is that I don't know but if anything it's it's highlighting to me that
56:47
there's a gap between us and that and uh highlighting what that Gap is one of the things I do is like I build on top of
56:55
generative AI so I can kind of see the Gap in ontological representations I can see what it can't do precisely and I'm
57:01
kind of getting closer and closer I think to to highlighting like the CH what what that creative or whatever it
57:07
is that makes us so special and why we're not going to be like overridden by
57:12
no matter how much data you throw this thing like I I sometimes like to say uh
57:17
it's sort of built in to like the scalability hypothesis so like natural language processing or machine learning
57:24
like B their statistic iCal models they're not they're not you throw all the data you want you're not going to
57:30
have perfect precision and if you had perfect Precision if you threw all the data and you trained your algorithms
57:36
perfectly what you would get at the end of the day is an ontology and so what we
57:41
do is we just add a little of the ontology up front in the training but that's not going to be able
57:48
to train itself so again all the way wrapped around to your question is there going to be a future for us doing this
57:54
absolutely I wish it wasn't case though because what we do is actually quite hard and I would I would be fine if like
58:01
they could we could throw enough data to make it go like make this this job go away but like I cannot see it and I'm
58:07
not at all doesn't frighten me at all if anything all the advances that are coming out are just kind of highlighting the
58:13
need and I think Gartner recognized that that's why we're at the center right like we weren't at the center of
Degrees, Skills, and Hiring Reality
58:20
their like hype cycle three years ago you know
58:29
that make sense I feel like I went on yeah yeah no no that makes sense yeah I I have some other questions but yeah
58:35
I'll let Mark go I get excited sometimes I'm sure you can yeah Mark hi yeah I just have
58:43
a purely practical question um so you say like if we if we want a job out
58:49
there doing this there are jobs to be had no problem good yeah what if
58:57
like what if I if I just have a master's degree like what level of degree do do I
59:04
want to have in order to get this job yeah so as I was saying so some of our undergrads have jobs um Masters have
59:11
jobs phds have jobs it really depends on what you where you want to see your career go so the advice I typically give
59:18
is a little ontology training goes a long way and if if you have like those
59:24
basic requirements like regardless of whether you have an education often the the the need for
59:30
hiring is so significant that hiring agencies will just kind of ignore degrees pretty pretty regularly if you
59:36
have the skill set and so um but depending on what you want to do in your career it may be beneficial for you to
59:42
get a master's or or PhD so if you want to for instance go into government and you want to go like up the food chain
59:49
which many of our graduates do PhD and the kind of virtue signaling that comes along with it it's it's just very useful
59:57
master's degree um that that opens a lot of doors too uh makes it easier to like
1:00:03
pay you at a higher salary for instance if you're working for contractors but really like at the end of the day though
1:00:08
it's the skill set like the we are at a point where the having a degree or
1:00:13
specific degree is less important than just being able to do the
1:00:20
work which is why like I mean I I'll share this story too one of our undergrads went to a conference with me
1:00:26
about ontologies and uh she ran into my old boss at John's Hopkins in the
1:00:31
Applied Physics lab in the bathroom and they were only in there for like three minutes and by the time she came out she
1:00:37
had a job offer she's awesome by the way the student's fantastic but like still like
1:00:44
it's crazy it's like I I say often I'm like what a weird world we live in they're doing like huge layoffs in some
1:00:51
areas of like like like some tech areas like massive layoffs like corre or
1:00:56
correcting after like Co hiring and whatnot and then here we're just philosophers just in high demand like
Practical Career Advice (GitHub, LinkedIn, Community)
1:01:04
what a weird world right so like on the Strategic Point
1:01:10
still like it seems like one of the best things someone could do would basically be to acquire training in formal
1:01:17
ontology from people who have these industry connections and then like to get one of these jobs do you need like a
1:01:24
letter writer like are you guys asked to to write letters for people or is it more like Word of Mouth kind of thing
1:01:29
often what happens is folks will well so I I give following three pieces of advice and they'll answer your question
1:01:36
so one is um come to these meetings there's like meetings I pointed out not not necessarily like the classes but
1:01:42
like just those weekly meetings although if you came to the classes they do the same because a lot of the students who
1:01:47
have enrolled right now this most recent semester are from government and they are here to learn what how to what to
1:01:55
look for when they're hiring so we have like half of our incoming class is from
1:02:00
the government and they're hiring people um or they're from con from companies that are doing hiring in this way as
1:02:06
well and so um just coming into classes you'll get FaceTime exposure same with like the the standing meetings you get
1:02:12
FaceTime get people to know who you are so that's one that's the first thing I always say the second thing is uh um
1:02:18
LinkedIn if you're not on LinkedIn get on LinkedIn and hook up with us so that we're all part of a network we will
1:02:24
promote you as you develop your skills and uh people that's more FaceTime and the third is uh if you're not on GitHub
1:02:31
then go to GitHub and get on GitHub and so GitHub is a if you're if you're unfamiliar like think about it as an an
1:02:38
analogy with like when you're writing in your word document at home on your local device and you're like no no no you hit
1:02:44
save and you like write some more and you hit save GitHub is like a way to do
1:02:50
all of that saving at each step in public so you make a commit they say in
1:02:55
everything you commit is saved at each point that way you can never mess up but it's important because in our circles
1:03:01
and this is not just just our circles but a lot of folks are in engineering circles are like this like you send a CV
1:03:06
in or somebody recommends you for a position the next thing they do is they go to see if you're on GitHub because they want to see what you do like your
1:03:13
CV is just getting you in the door me recommending you is just opening the door but like they still want to see if
1:03:20
you can do the work and I tell my students all the time I'm like get on GitHub because they don't know what you're doing otherwise
1:03:26
like hiding in a room and thinking hard about a problem is not going to show them that you're working they have no
1:03:31
idea who you are so go on GitHub and just create and what what's good about going on GitHub is you have like a
1:03:36
little like history like every day you're on you have like a little Green Dot that highlights like brighter and
1:03:42
brighter so they can just look and see oh this person works pretty regularly they can see the projects you work on they can see the kind of work you do if
1:03:48
you want to know more about the details of actually what it means to work in GitHub in this space come to the
1:03:53
meetings because we we like I walk people through how to engage in GitHub
1:03:59
and how to make contributions to the community um and it serves both purposes one to help the community and too to
1:04:05
like help their resume can you tell I'm afraid of of
1:04:11
this community fan like I I really I want come help okay I have another question then
1:04:20
um so he said what they really want to see is that we're doing the work that we're putting the work in
1:04:28
um I guess not having done any work in implied autology right like for any kind
Tools of the Trade (Protégé, TopBraid, etc.)
1:04:34
of customer or anything like that um when I open up GitHub um what is it that I do like are
1:04:41
there like resources online or do y all provide resources that have like example projects or example ontologies that you
1:04:47
can then like what is it that that I would be doing in GitHub to show them that I'm putting in the work if that
1:04:52
help if that's makesense let me let me illustrate I'll just okay show you it's
1:04:59
a great question I'll show you what some of our uh some of our students are doing okay
1:05:07
here let me share my screen you see my screen you should see
1:05:12
a picture of me making a weird face yeah old photo okay so uh I'd
1:05:19
mention the common cor ontologies it's one of the ontology sues that we work on pretty regular it's pretty widely used
1:05:25
but you see um so here on this is a
1:05:30
GitHub repository this is where like the the the the ontology artifacts are stored so people can download them if
1:05:37
they want like if you went to Source you'll see the ontologies here let's see where they on the modules there's like
1:05:43
an agent ontology an artifact ontology and this is just like this is the the format they're put in um but really like
1:05:51
what I want to highlight here is there's issue trackers like if you have issues if you have updates if you have things you want changed or just something
1:05:57
you've observed that you think is could be fixed or corrected or made better in the ontologies you can you can open an
1:06:03
issue on GitHub and uh let's see so this is one of our students um Alec he he is
1:06:10
identified I haven't read this so I I hope it's it's reasonable but he's he's looked at the definition and he is
1:06:18
raising a complaint about it and this is one of the developers of of um CCO the
1:06:23
common cor ontologies and he is is uh engaging with him and giving him some guidance and here's one of our other our
1:06:30
contributors and so this if when I'm hiring this is what I'm looking for I'm
1:06:35
like is that okay good good good good and you'll see a lot of our students Greg over here our former student
1:06:41
actually Greg's offered a lot of stuff we have uh Neil like folks like this so
1:06:46
these are all these are all familiar faces to me these are people who have done this there's also a discussion forum where you can do something similar
1:06:53
that we SE we separate discussion from the issue isues and the issues are like actionable like we can fix things now
1:06:58
discussions are like more open-ended like if you have a question about the nature of viruses or something it might
Final Thoughts: Philosophy’s Unexpected Power
1:07:04
go on the discussion board you'll see a lot of the philosophical stuff come out on the discussion board which is why kind of we kept it aside still valuable
1:07:11
to have but you know like that you that's also contribution right like you're moving the discussion forward and
1:07:17
you'll you'll find like the philosophical background coming out there like when I'm on there I'm premise
1:07:24
conclusion looking like do disjunctive reasoning I'm highlighting fallacies I
1:07:29
get a little nerdy but but yeah um like I said when I'm when I'm when I'm hiring
1:07:34
people that's what I'm looking for I I want to see like the depth of their engagement um and I'll I'll share to one
1:07:40
of my uh one of my mentees from Northwestern he uh he raised one issue
1:07:47
on one ontology Forum on GitHub uh it was a good one he was like hey you're
1:07:53
defining assay in a in too broad of a way and here's a proposal for how to fix
1:07:58
it one week later they made him a job offer and he has been working at La Hoya
1:08:03
Institute in the biomedical wing for like two years now like one one issue
1:08:10
and he's not the only one that's happened like with some other students um not my mentees but like this this
1:08:15
happens not infrequently like the the field is kind of if you have the philosophical SL engineering like you
1:08:23
have the philosophical background and the engineering mentality which is not that hard to get especially if you're
1:08:28
not if you're coming to the the meetings we we'll get you there um the field is
1:08:34
ready yeah that that's that's helpful and I have one more small question do
1:08:40
you have um uh it's like this is just because of
1:08:45
like my life right now we just had our first child very young congratulations that's awesome yeah yeah and so like
1:08:50
doing things that are scheduled right now we don't really have control over that the the kid kind of determines you
1:08:57
know when we're available and stuff right now um if you had to point to like a text or
1:09:04
something like that that someone who wants to get involved in this could could work through right just to
1:09:10
familiarize themselves with like the language um and you know how to you know but when I get on GitHub right like how
1:09:16
I need to some way I need to know what they're talking about right so like AB yeah yeah so do you have any recommendations for like text or
1:09:22
anything like that so I my fir first send me an email and I will send you
1:09:27
like I have a a boilerplate email for this just this question and I'll send you that okay who wants it I'm happy to
1:09:34
send this out but uh but I'll tell you right now like the main text to read is called semantic web for the working
1:09:41
ontologist and you can find it online like the second edition so it's the most recent Edition it basically gives you a
1:09:46
lay of the land just like at a high level tells you like the tech that we use the sort of why we use it what you
1:09:52
can do with it really gets the jargon down and when I send you the email I'll also send I don't know if you're
1:09:58
familiar with anky um this kind of flashcard software it's really lightweight I have an an SL like
1:10:05
flashcard deck um for that book as well as several other books which I'm happy
1:10:11
to share with you like just again all these resources you can have in fact now
1:10:17
that I'm saying this out loud I should put that anky stuff online because every I'm gonna put it online after this and
1:10:24
like highlight it folks can use it as well but yeah I'm happy okay yeah cool I'll send you an email
1:10:30
[Music] thanks um someone related question John
1:10:37
about like the kind of workflow involved in these projects so are people typically hired by a contractor or a
1:10:45
company for a set project and then when the project is over they just have work experience and they have to get another
1:10:52
job or like are people hired as like permanent employees of company and like they're laid off only if the company
1:10:57
starts you know going through financial pressure so often in in my experience often what happens is uh you if there
1:11:06
are internships that work like you've described with they kind of fixed time frame and they may or may not be
1:11:12
continued based on how how good or what the nature of the work is or whether there's funding there's Contracting work
1:11:19
um which is is in some in some areas like it works just like youve described but in here in our area Contracting work
1:11:27
is typically um for set projects but when those projects are over you're so
1:11:33
valuable because of the skill set that you have that there are just other projects for you to work on unless the
1:11:39
company itself is just tanking they will keep you on I've I've known several cases of ontologists who have just been
1:11:47
kept on staff um and paid throughout for other projects because the company knew
1:11:54
that like in six months they were going to get another ontology contract it was just so much it's so much less expensive
1:12:01
to like let you go and then try to hire you again than it is to just keep you on
1:12:06
and so that's what's happening more often than not but really like the mo most regularly what's going on is that
1:12:11
folks are getting hired into full-time positions um that are not Contracting work but like actual just you know paid
1:12:19
positions like you would in like a university or something but these are often in government so it's a nice cushy
1:12:25
government jobs so government agencies many government agencies are really interested in hiring ontologist inhouse
1:12:33
partly because they're tired of getting like vendor locked where they then they they're really keen on like having folks
1:12:40
in house that can do the work so there's a lot of folks in government who are like keen on hiring up people for this
1:12:45
and that's that's like a position if you pass the first year then and you're not like super high like political appointee
1:12:51
level it's really hard to lose your job yeah so yeah some options um I can I
1:12:59
guess I can also say something about the banking side so like Finance industry is hiring a lot of ontologists as well I
1:13:04
know I have some close friends who were working there and those jobs are fairly secure and even if they weren't uh from
1:13:10
what I understand you know as you're part of the network it's it's hard to
1:13:15
let you go right like I can always move you over here you can do this so you can do that and the skills we have um are
1:13:22
pretty marketable in other areas right like of course skill set is not just like understanding what an ontology is
1:13:28
in the tech it's like strategic conceptual thinking which any any
1:13:34
manager will tell you is something that's very challenging to train and something that's highly valued as like a
1:13:41
leader a sub manager like for for Creative projects like they they can
1:13:46
find a place for you if you ever get in a point if you
1:13:51
enter this field you ever get in a position where you're like I think I might is my job you tell
1:13:57
me and we will make sure it doesn't happen or we'll make sure it happens and you go to somewhere
1:14:03
better yeah yeah Mark so I'm following up on Josh's
1:14:10
questions it's so the picture I had before Josh started asking questions uh
1:14:15
sorry Josh tigor started asking questions was that you just okay I I I'm
1:14:23
I'm done with philosophy tomorrow tomorrow I want to start working in ontology that doesn't sound like that's
1:14:28
what happens it sounds like there's a Year's worth of retooling I have to do I wouldn't even say I would even so it
1:14:35
depends on where you are in your philosophical background really so I would I wouldn't say give a philosophy I
1:14:41
do philosophy all the time uh I love it if I in fact I'd be loed to do what I do
1:14:46
if I'm not doing philosophy but that philosophical skill set the thing you've developed that is a big reason why our
1:14:53
students are getting hired so so I I I say sometimes like the text side is very easy to get it's it's not conceptually
1:15:00
that challenging and I don't I and I say that I mean that all seriously like read that semantic web for the working
1:15:06
ontologist book it's not that long because there's not that much there's not much to learn but what is hard to
1:15:11
learn is the wisdom that comes from Deep conceptual thinking about dense material
1:15:16
and like thinking a high level concept like logically and that is just not something that most people outside of
1:15:23
our Discipline Do and you'll see that again and again and again as you work with folks what seems so obvious to you
1:15:30
is not I once had a long conversation with the head of knowledge representation at a huge company that I
1:15:36
can't name and she was telling me that like over six months they had been struggling over the following problem
1:15:42
they were they were trying to like model they were trying to model the case of when a consumer goes to their website
1:15:48
and they want I'll say they want a candy bar but they don't want a specific candy
1:15:54
bar she was like I don't know how to model that none of us have figured out how to model that maybe 6 months is a
1:15:59
stretch may like two months they they've been struggling over this so like I said I said
1:16:07
listen just you just have a a class candy and then you have sub classes for
1:16:13
the types of candy like Snickers Kit Kat and then when somebody wants a piece of
1:16:19
candy but not any specific piece of candy it's outside all of those suglasses but there's an instance
1:16:25
outside of those sub classes you don't know what it is but that's it and she
1:16:30
thought and she paused and she was like an uncomfortably long silence and then she looked at me and she said oh my God
1:16:36
I think you just solved this problem but it probably seems very obvious we probably knew what I was going to say
1:16:42
before I finished the senates right but like they're just not trying to think that way much like we're not trying to
1:16:47
think in whatever like specific like engineering strategies or languages that
1:16:52
they use we have our own special skills right but that wasn't so the question you answered was uhuh why why choose
1:17:01
philosophers great my question is how much work do I have to do to get into
1:17:08
this like when I start applying for those jobs at LinkedIn I you can Circle that bit that says philosophy but I
1:17:13
didn't look carefully what the rest of the requirements were yeah yeah read that book that semantic web for the
1:17:19
working ontologist so I was trying to answer that part of the question too right like so that book read that book The Tech is not that hard getting the
1:17:26
language down not that hard most often what happens is folks who read this book they'll come talk with me they'll come
1:17:31
to these meetings they'll go learn the actual details on the job but what they can't learn on the job
1:17:39
is the philosophical background and that's the stuff that's that's one of the again one of the main reasons they're getting hired so they can pick
1:17:46
up the tech stuff and this is not uncommon in like engineering honestly like it is not uncommon that you have to
1:17:52
come in and learn a new stack like that happen happens again and again they usually give you like a month to get up to speed wherever you are this is not
1:17:58
not unfamiliar territory but they did hire you even in those cases for some specific way of
1:18:04
thinking like like in machine learning thinking or NLP or something and for us is philosophical thinking so so I don't
1:18:11
need to take classes and I don't need to get a certificate I just need to read that book and then I yeah read that book
1:18:20
maybe come talk to us get your face in the right faces get a GitHub account so they know when they're looking around
1:18:26
they they they want to like see that you're actually doing stuff right and like you do those things LinkedIn of
1:18:32
course but it's all about like getting your face on the right faces that minimal understanding of like the jargon
1:18:38
and then playing around on GitHub so that they see you're serious you come join us
1:18:46
okay you'd be surprised too I I those three things every time I've recommended people do those three things like my
1:18:53
students the ones who do those three things get jobs like almost immediately and then the ones that just do two of
1:18:58
them they're like how come I'm not getting a job like I told you what to do just do those three things but it's
1:19:05
really kind of it's well I mean like if I went to GitHub right now if I went to GitHub right now I
1:19:11
wouldn't know what to do on GitHub you know you need to my work you know they'd be seeing is composition real you know
1:19:18
is comp is composition fundamental right that's not what they want to see right that sounds like a discussion board post
1:19:25
okay that sounds like I mean honestly like uh there are there are debates over that in our field like composition
1:19:31
special composition question it comes up not infrequently uh we it sometimes comes up directly like that sometimes
1:19:37
doesn't it comes up in other other garbs you'll see like Engineers talk about it in different ways it's structurally the
1:19:42
same sorts of questions you'll you'll be surprised as you start exploring if you're interested in exploring you'll be
1:19:47
surprised at how many philosophical like familiar philosophical puzzles start emerging like shipus
1:19:55
like natural versus unnatural properties like yeah and you're well you're well
1:20:00
equipped to like clear up confusion and that's
1:20:05
valuable I have another question right so I read this book um I I go to GitHub
1:20:12
I try and answer some questions get involved in some discussions um I come to the meetings
1:20:20
um when I think about applying to a job on something on LinkedIn
1:20:26
I immediately start thinking well there's there's going to be some kind of um platform or something that I need to
1:20:33
know how to use right like GitHub is a kind of like information repository right where we can get there sit there
1:20:40
and ask questions and get answers um are there any like essential like I don't I
1:20:47
don't know any other word than platform that you know that you use to build ontologies and navigate ontologies that
1:20:52
I would need to become familiar with so different groups use different tools um but if you were looking if you were
1:20:58
looking um so uh for some to to check out so there's this Protege editor
1:21:04
that's the Stanford group creates it's open source it's uh it's it's a way to like visualize linking parts of
1:21:11
hierarchies to other parts of hierarchies which kind of what we do there's also this top braid composer
1:21:16
that's that's another common one there quite a lot of tools out there many of these covered or at least discussed in
1:21:22
that semantic web book so they'll make okay um okay and often though that is
1:21:28
sort of I mean well it's good to have those skills it's like good to know how to use these various platforms just like
1:21:33
it would be in any other field toolkits like a lot of the training happens on on site right um
1:21:40
because who knows if you're using top braid or if you're using some microft
1:21:46
develop tool like a lot of groups have different tooling that they want so like a customer they'd be more
1:21:53
than willing if they if they notice you have this skill set this valuable skill set they'd be more than willing to say
1:21:58
okay I'm willing to try you on this project and let you just kind of learn on the go how to navigate these
1:22:04
platforms and stuff oh yeah I I started working at John in the Applied Physics lab while I was a graduate student I'd
1:22:11
never used top braid before they used top bra and I was like okay I guess I'll
1:22:16
use this the tech though is so it's lightweight it's not hard to figure out it took me a little bit but I had to
1:22:22
learn like I learned things like using Jenkins to make builds in the background bit bucket and Source tree to like
1:22:28
organize like a lot of jargony stuff right I learned all of this working there because that was how their infrastructure was but I knew none of it
1:22:37
before but you know I knew what I think deeply and logically about me and that's
1:22:44
call a philosopher right okay that's encouraging to hear I like
1:22:52
to I like to think of it as they're like I mean they're kind of hiring us for a wisdom and I think of philosophy is you
1:22:58
know study wisdom like we're exploring wisdom right and it's not a specialty it's not something you go like get an
1:23:03
electrochemical degree in right like we say we get philosophy degrees huge right
1:23:08
like covers so much wisdom is Big it's not a subdiscipline and so that that's hard to train hard to get hard to master
1:23:16
worth it worth hiring I I'm emphasizing this because a
1:23:22
lot of times I talk with philosophers and where you know I know what the Market's like right it's terrible right
1:23:29
I had I had no hopes about even attempting I wasn't in interested at all in going to academic Market but but I
1:23:36
you know it's so it's such a such a turnabout right like in ontology circles
1:23:41
I'm head hunted like people come at me with huge offers and I'm like you know great like it's such a weird feeling
1:23:48
like I'm a philosopher and they're coming at me for largely for the philosophy background which is just it's
1:23:54
weird right what a weird world we live in