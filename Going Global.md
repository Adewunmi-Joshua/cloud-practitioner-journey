# Going Global

Remember I mentioned **regions** and **zones** in my cloud basics documentation.  
We will need them in this section to properly understand what *going global* means.


## Region

A **region** is a geographical area (usually a country or part of the world) where cloud data centers are located.

Each region is independent and designed to keep services running smoothly.


## Availability Zones (AZ)

**Zones** are specific spots within a region where those data centers live.

Every region has a few of these zones, and they team up to make sure things stay up and running and to keep things fast.

Each zone has its own:
- Power
- Cooling
- Networking


## Example

Let’s say **Nigeria is a region** (this is just an example).

Inside that region, there are different **zones**, such as:
- Zone A (data center 1)
- Zone B (data center 2)
- Zone C (data center 3)

All these zones work together so that if one zone has an issue, the others can still deliver resources without interruption.

## What Does Going Global Mean?

Going global means deploying your resources in **different AWS regions** to increase availability and serve users worldwide.

This helps your application reach users closer to their location and remain available even if one region fails.


## Example

Imagine you love buying tea from a restaurant in your home country.

As time goes on, you relocate to another country and expect to see that same restaurant, but unfortunately, it is not there.

One day, you are told that the restaurant has expanded to your new country and plans to expand to even more countries.

What that restaurant just did is called **going global** — making its services available to more customers worldwide.


## Benefits of Going Global

- Improving performance, availability, and reliability
- Reducing distance between users and your application
- Serving users from different countries

---

## Deploying in Multi-Region and Multi-AZ

### Multi-Region Deployment

Deploying your application in **multiple regions** increases availability.

If one region fails, another region can act as a backup and continue serving users.

This is commonly used for:
- Disaster recovery
- Business continuity
- Global applications


### Multi-Availability Zone (Multi-AZ)

Multi-AZ deployment means deploying your application across **multiple availability zones within the same region**.

This improves:
- Reliability
- Fault tolerance
- Application uptime


## Example to Clarify Things

Imagine you only have **one generator** providing electricity to your house.

If something happens to that generator, there will be no light, and everyone in the house will know.

Now imagine having **four generators** designed to assist each other.

If one generator fails, the others take over without interrupting power.

That is what deploying your application across **multiple availability zones** looks like.

If one zone (data center) fails, another zone in the same region continues serving traffic without users noticing.

If the **entire region** fails and you are deployed across **multiple regions**, another region can act as a backup.

## What CloudFront Does

CloudFront is AWS's global network that delivers websites, videos, and other thing super fast. It does this by saving copies (cache) of your content closer to your users, which makes things load quicker.

## What's an Edge Location?

Think of an edge location as a small data center specifically built to get content to people faster. It stores temporary copies of content so it's right there when someone asks for it.

## Example to Clarify Things

Let's say someone in Rwanda wants to watch a movie on Netflix.

If Netflix kept all its movies really far away from Rwanda, that person would have a slower experience.

That's where edge locations help out.

To fix this, Netflix would put a copy of that movie in an AWS edge location near Rwanda. This means when the person in Rwanda hits play, the movie doesn't have to travel a huge distance, so it starts playing almost instantly.

## What Low Latency Means

Low latency just means there's no annoying wait time when you ask for something.

Like when you're playing a video game you definitely don't want any lag, right? AWS is built to cut down on those delays.
