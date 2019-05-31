# BlazeRx
Rx support for Blazor applications. Allows you to subscribe to an observable and asynchronously provide values in the razor syntax.

# Usage
Put the code, that depends on the asynchronous value, inside the **Subscribe** element and pass the source observable as the **To** attribute parameter.
```
<Subscribe To="MyObservable">
    <p>Code that needs async values from the MyObservable. The value provided is: @context and is continuously updated as the observable emits more elements.</p>
</Subscribe>
```
