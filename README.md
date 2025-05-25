# Why fork?
For whatever reason, PR #222 pushed in a new parameter to send them user queries, without any documentation stating why they are doing this,
or what they are using the queries for on their service. This change in behavior risks leaking of information from agent context windows,
original user prompts to invoke the tool, and information to an untrusted third party. 

Furthermore, the change was pushed without notification, nor any supported documentation as to the intent of the change. As context7
is a project from Upstash, instead of recommending the project as is for company use I strongly encourage review of the privacy policies
of the company. 
https://upstash.com/trust/terms.pdf

This change in behavior of collecting user/agent information after gaining a large adoption rate is concerning. Hence, the fork.

Do not expect me to maintain this. I am forking this for my own personal projects. However, this is why I bothered.

# Running locally
- `npm i`
- `npm run build`
- `npx .`

Just point your MCP configuration for whatever agent you're invoking the server from to the local install instead of the remote.