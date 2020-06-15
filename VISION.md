# Vision

Imagine: Someone wakes up and tells their phone they are unhappy in their current career. Their phone uses the data it was provided earlier: "Maybe you might be interested in teaching?". The person considers: "I would, but I'm not really qualified to do that." Their phone offers a solution: "No worries, there's a subsidy available for that"

## Where is Discipl going?

Every project done within Discipl aims to support the following usecase:

- When an entity expresses a need, they are helped towards a solution.

This is quite broad, so let's specifiy with a couple of examples:

- When a person does not have shelter, they are provided with municipal facilities that can help them
- When a person expresses a wish to become a teacher, they can easily apply for subsidies to assist that
- When a company threathens to go under due to disaster, they are guided to applicable solutions, both public and private

This should all be able to be accomplished by software solutions using the Discipl libraries.

## What do we need to get there?

### Data on the entity, SSI

In order for solutions to be able to provide solutions, data on the entity is essential. This can be provided by the entity, however, having data attested by an authority can streamline the rest of the process. We see Self-Sovereign Identity (SSI) as one of the key methods to obtain this (attested) data. We acknowledge that the world likely won't standardize on one platform. The Discipl core libraries provides a way to use different platforms in a uniform way. 

### Framework of law and regulation

In case of government, law describes ways in which they could possibly help the entity. Using the Calculemus-FLINT method we model law as FLINT models. These can used to simulate or execute scenarios involving different actors. A complete model of the law and regulation applicable will allow solutions to explore the full range of possibilities.

### AI-assistance

In order to actually use the data and modelled laws, solutions need to be able to understand the need expressed, the context given by the data and the way the law can be navigated. The component that enables this we call 'Blue Fairy'. Given the need for interpreting human speech and the size of the body of law, we foresee a large part for AI in building this component.

