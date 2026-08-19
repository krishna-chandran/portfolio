---
kind: paper
title: "From a slat actuator to a farm fleet: the career, on the record"
date: 2026-08-19
dek: "Aeronautics, enterprise AIOps, a Mazak spindle, airport tractors and autonomous farm machines — one habit, told in order."
kicker: "Paper"
dateline: "Los Angeles"
categories: ["Career"]
---

LOS ANGELES — Krishnakumar Chandran works in artificial intelligence, physical AI, robotics and autonomous vehicles. The present dateline is this city. He is out of Agtonomy; that role, from March 2024 in South San Francisco, was the last full-time card — data paths from autonomous farm machines back to a cloud growers and engineers could use. The file behind that sentence is longer than a job title: a first degree in aeronautical engineering, a decade of production software, and a habit of making a system observable before asking anyone to trust it.
<!--more-->

{{< well kind="lead" src="images/krishna.jpg" prompt="Portrait, 16:9, Cincinnati, natural window light, engineer in plain clothes." caption="Krishnakumar Chandran. Formal training in aerospace; the rest of the paper is production." />}}

What follows is the public record — education, projects and the jobs in between — written as a single story. Each of those events also has its own page in this paper, dated and filed in order. Salaries, visas and private reasons are not in this file.

What separates the file from a typical software career is the seam. Most people specialize in software AI or in physical autonomous systems. He has sat both, and applied the same three tests — reliability, scalability, observability — to a ServiceNow queue, a CNC spindle, a ROS bag and a farm tractor. The aerospace degree is why the argument includes how a system behaves in a room that moves.

## The nut graf

The career has three rooms. The first is aerospace: wings, actuators, CATIA, a journal note on the Tejas. The second is enterprise AI: ignio at Tata Consultancy Services, first in Chennai and later in Farmington Hills, walking data centers from a ticket queue toward a machine-first model. The third is physical AI: a Mazak spindle that had to confess early, airport baggage tractors that had to name what moved, and a farm fleet that had to report what the field did.

The through-line is not a stack. It is the same brief, asked of different machines: observe, score, recommend, do not pretend the average case exists.

## Timeline

### 2010–2014 — Chennai, still an airplane

He is from Erode, Tamil Nadu. Primary and secondary school were at Navarasam Matriculation Higher Secondary School. From August 2010 to April 2014 he read aeronautical engineering at Rajalakshmi Engineering College, affiliated to Anna University. The GPA was 7.6 on 10. The syllabus was mechanics, flight dynamics, aerodynamics, CFD, structures, composites, propulsion and avionics — wings, not web forms.

EDS Technologies, a Dassault Systèmes platinum partner in India, certified him on CATIA V5 primer and advanced courses: parts, surfaces, assemblies. In 2013, with Vijay S, he presented “Application of Artificial Intelligence in Unmanned Aerial Vehicles” at a national seminar at C. Abdul Hakeem College of Engineering and Technology, Vellore.

The first industrial problem was already physical. On the Tejas, a slat actuator was developing play after about 300 operational runs. Unwanted motion damaged the parts around it. Hindustan Aeronautics asked for a root cause and a fix that could be proven. He derived approximate equations for the existing actuator under load, proposed a redundant link to spread that load, modeled both configurations in CATIA V5 and took them to ANSYS. The paper, with Manikandan C and Niranjana S, appeared on 1 October 2014 in the *Journal of Basic and Applied Engineering Research*: “Conceptual design and analysis of link for arresting slat actuator play in TEJAS aircraft.”

Then he took a software job.

### 2014–2017 — TCS Chennai, ignio’s night shift

From September 2014 to September 2017 he was a software developer at Tata Consultancy Services in Chennai, on Digitate’s ignio AIOps: network automation and the quieter work of event triage, incident prediction and automatic resolution in a data center.

He wrote about 160 ignio scripts for network administration, covering some 90 percent of those tasks, and built Service Operations for L2 and L3 switches, firewalls, load balancers, F5 and Infoblox. The appointment ran through July 2017.

One outside engagement in 2016 was Nielsen Media India: NetBackup automation and backup analytics on ignio. About half of the manual reporting and IT operations time went away.

The work was not glamorous. It was the first draft of a career that would later treat a tractor’s bag file with the same respect as a ticket queue.

### 2017–2018 — Cincinnati, control theory and a shop floor

In August 2017 he enrolled for a Master of Engineering in aerospace at the University of Cincinnati. He finished in December 2018 with a GPA of 3.5 on a 4.0 scale, on a 50 percent graduate scholarship, and he did not leave the city. The focus was unmanned air systems, analytical dynamics, modern control and artificial intelligence, with decision engineering, intelligent data analysis, big data analytics, and a pair of innovation courses on the side.

The internship sat inside that year. From July to December 2018 he was a full-stack engineer at the Intelligent Maintenance Systems laboratory at UC, on a Mazak-funded project: predict CNC spindle failure before the floor hears it.

A vibration sensor and a current sensor went on the machine, into Advantech acquisition on an industrial PC. Data was taken when the machine was new, dry of lubrication, imbalanced, and with a broken spindle. FFT features, principal-component reduction and logistic regression won the classification. He wrote the path from experimental notebooks to production Python and Flask, and a web face for a health score from 0 to 100. A score below 50 meant maintenance; below 30, the machine was not to be used.

Mazak put the spindle-health monitor into its machines. In September 2018 the work was shown at IMTS in Chicago, with Mazak and the IMS lab on the banner. The university [wrote it up the following January](https://www.uc.edu/news/articles/2019/01/n2063491.html), naming Hossein Davari and Vibhor Pandhare on the same bench.

In 2019 he placed as second runner-up at UC’s IQ E-Pitch, a Lindner College of Business elevator-pitch contest, with a sport-analytics idea that used AI on a soccer match.

### 2019–2021 — Farmington Hills, machine-first

From July 2019 to September 2021 he returned to TCS as a product architect for ignio AIOps and ignio AI Digital Workspace. The card was end-to-end: understand the problem, read the existing landscape, design and configure the solution, coordinate offshore teams, write the migration and integration plan, and stay through go-live and change management. He wired the product to ServiceNow, SolarWinds, AppDynamics, Office 365, Active Directory, email and CyberArk, put chat-based tickets on Veeva Vault user access, and sat AI and cognitive use cases on ignio itself. A Kafka–ELK log stream cut debugging time by 90 percent.

Mercedes-Benz Financial Services was among the accounts: a data-center deployment that walked IT servicing from a manual-first incident habit to a machine-first delivery model. Belk, Toyota Motors North America and Astellas sat in the same years. The ignio product itself is in use at more than 260 Fortune 500 and Global 2000 shops; his piece of that story was the network and Windows Server automation from Chennai, and the architect who sat with the client.

### 2021–2023 — ThorDrive, one job, two tracks

From October 2021 to March 2023 he was an estimation and tracking engineer at ThorDrive, on autonomous tractors meant to move baggage at an airport. The title on the card did not split. The work did: perception on the apron, and a data platform that had to take in the tape.

He wrote a FLIR thermal grabber as a ROS node, lidar segmentation and a lidar tracker, and fused five RGB cameras with two lidars. YOLO v4 was trained for pedestrians, cones, K-loaders and airplanes. PointPillar and mmdetection3d were pushed for 3D detection. Ground segmentation followed the papers. Tests ran with the airport’s team at Cincinnati/Northern Kentucky International — in the ThorDrive years, not earlier.

The bags had nowhere honest to go. He designed an internal platform for petabytes of ROS bags, live telemetry and operator logs, raising data capacity by about 250 times, and built search, visualization, snapshot, parse, label, query, clip and download. Data-workflow time improved by 91.4 percent. ELK pipelines against the vehicle computers cut crashes by 90 percent. The career file says he built that infrastructure himself. The conventional loop — a person on the apron — became a cloud query. Productivity, on that file, rose by more than 90 percent.

### 2023 — Protekk, a plan for one student

In 2023 he cofounded Protekk Web Technologies LLP and sat with a client that wanted an education product, not a brochure. The brief was public-school students and a plan that belonged to one child rather than a classroom average: dynamic assessment across subjects, student-specific lesson plans, and an AI recommendation system meant to move a learner faster through what they already knew and slower through what they did not.

The company was a year of software for schools after a year of software for tractors. The habit was the same: observe, recommend, do not pretend the average child exists.

### 2024 — Agtonomy, a fleet that reports

On 12 March 2024 he joined Agtonomy in South San Francisco as a software engineer in data analytics. He later left that role. He wrote custom C++ on the tractor, Docker images, and pipelines on Vector, InfluxDB, Timestream, OpenSearch, S3, ClickHouse and Kinesis. gRPC, Protobuf, sockets and REST carried the traffic. A vehicle-state agent published snapshots to Redis. Vector ran on Fargate and ECS with autoscaling. When the store changed, he moved InfluxDB to Timestream, InfluxDB to S3, and S3 to ClickHouse.

The architecture was drawn for as many as 300 vehicles talking at once. Stream processing pulled metrics from terabytes of raw telemetry. Backend APIs fed the boards a grower or an engineer opened. On the record, he played a key part in taking a fleet that had been on the order of twenty machines toward 250. Agtonomy has automated Bobcat AT and CT machines and the Kubota M5N, in vineyards and olives, for mowing, spraying and scientific collection. During this period the company closed a Series B, took a partnership with Kubota, and put the work on a stage at CES 2025, FIRA 2025 and CES 2026.

The argument for the farmer is older than the stack: labor is short, the row is long, and a tractor that cannot report is only half a robot.

## What he is after

The next problem on this file is not a particular employer. It is a digital platform for American companies already running rooms where people, AI systems and robots share the work. Medium and large estates have legacy systems welded to old processes; a small shop can adopt a new model in a week. Those estates need a way to hook the old systems to modern AI, watch an end-to-end process, and see whether a gain is real.

As language models, autonomy and robots take the repetitive layer, project boards stop describing how work is actually made. Junior roles thin out. New ones appear around supervising and validating the stack. Fewer paths remain for a new engineer to get time on a live system. The platform he describes would treat human, AI and robotic contributions as one operational file — throughput, cost, constraints, competency — identify whether a stall came from a skill gap, a machine limit, inventory or something outside the building, and feed that file back as on-the-job training. Automation, on that argument, should not only replace a person. It should keep a way to become one.

{{< well kind="inline" src="images/krishna-profile.jpg" prompt="Mug, 4:5: a second portrait, three-quarter, quieter." caption="The profile shot. The paper uses it when the lead is a machine." />}}
