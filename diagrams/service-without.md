```puml
@startuml

node "Kubernetes Cluster" {
    node "Node 1" {
        component "Pod Client" as client
        component "Pod A" as poda1
        component "Pod ..." as podb2
    }
    node "Node 2" {
        component "Pod A" as poda2
        component "Pod A" as poda3
        component "Pod ..." as podb1
    }
}

client --> poda1
client --> poda2
client --> poda3

@enduml
```