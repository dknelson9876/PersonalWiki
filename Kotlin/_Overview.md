# Overview
- `ViewModel` is the Kotlin architecture practice for separating data from UI
- `LiveData` is the lifecycle aware way to let a UI class subscribe to changes to data in a `ViewModel`
    - *Data Binding* is the strategy that allows us to reference LiveData objects directly in our xml views to take shortcuts and remove extra code