# Provider Simulator - design specificaiton 
- Provider 
    - has basic set of fields 
    - Provider has set of capabilities 
- Capabilities 
    - can be added or removed thru simple configuration files 
    - are considered as "addons" to a provider. 
    - exposes `DataGeneerator` interface 
        - `DataGenerator` takes one paramenter `scenario` and returns `JSON node`
        - Quesion: How do we handle the user associations with the data?  
    - listens to events 
        - `onEvent` they react and change state of the data 
- CapabilityDecorator 