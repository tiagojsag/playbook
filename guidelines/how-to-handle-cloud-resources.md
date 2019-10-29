# How to allocate cloud resources

This guideline covers the steps you should take should you need a cloud resource, like a server to host a project, a file bucket, a Carto/(something else) account, etc.

## Project resources

Most of our projects require some sort of hosting to run on, be it a server to run code on, some hosting-as-a-service like Heroku, and S3 bucket to store files etc. More complex projects may need certain services, like Carto, Google Earth Engine, Transifex, etc.


### Resources owned by the client

While there are multiple ways in which these resources can be provisioned, the recommended way is to talk with the client and have them own these resources themselves. This carries a series of advantages both to us and the client:

- If they own their resources, there's no transfer cost or delay for either us or them, should they decide to hire another provider in the future.
- They own the service accounts, much like they own the code/design/etc we build for them.
- Should they already have a cloud infrastructure, they can consolidate to cut costs.
- For the duration of the project, we are available to have technical ownership of these resources, so we'll still set up resources as needed, even though they are not owned by us.
- Billing is handled directly between the client and the service provider, without us being needlessly in-between the two. 


We should be clear and transparent when communicating the need for these resources with the client, as these costs can appear as unexpected to some clients, and their internal budget for the project may be restricted:
- We should discuss with the client why this resource is needed.
- We should, when possible, present alternative solutions to the problem, and provide a recommendation based on our expertise, as to why a given solution is superior to the others.
- We should provide an estimated cost of the service, clarifying that it will be charged by a 3rd party, over which we have no control.
- We should be upfront about the cost of these resources.
- We should clarify if the cost is temporary (ie: staging servers) or "permanent" (ie: production servers).


Given that setting up these resources can be a quite technical process, we can help the client with the practical steps, by:
- Creating the necessary service accounts for the client, using their data.
- Setting up the resources for them.
- Providing links or other resources that helps them carry out the process themselves, should they wish to.
- Joining them on a call, screenshare, and guide them step by step if they prefer to do these steps themselves.
- Provide links or other resources covering any post-delivery maintenance tasks they may need to carry out (or advise them to hire external help, should you think that's the best option for them).

Once the development phase of the project is over, don't forget to backup and delete any staging resources that may have costs associated, so we keep our client's bills as low as possible.


### When "we" are the client

For some projects, we are our own client (for example, grant-based projects), so the above doesn't apply. For those situations, Vizzuality has its own set of accounts on Google, AWS, etc, that we can use to host and support our own projects, keeping in mind the following:
- Our accounts can have resources allocated to multiple projects, so be sure to name and/or tag the resource in a way that makes it easy to match it to its corresponding project.
- For the same reason, clearly identify if a resource is a staging resource, and can be deleted once the development phase is over.
- On the project documentation, clearly identify these dependencies on external services, should we need to make adjustments in the future (ie: renew api keys, migrate accounts, account spring cleaning, etc). 
- Talk with the PM so the cost of these resources can be accounted for.