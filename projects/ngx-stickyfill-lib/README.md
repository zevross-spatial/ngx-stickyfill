# ngx-stickyfill

An Angular 2+ (tested in Angular 7) directive for easily using stickyfilljs, a polyfill allowing one to use position:sticky in browsers that don't yet have sticky support.

# Installation
First install the necessary stickyfilljs dependency:

```
npm install stickfilljs --save
```

Then you can install ngx-stickyfill:

```
npm install ng-stickyfill --save
```

Then add the ngxStickyfill module to your app or shared module:

```
@NgModule({
  declarations: [
    AppComponent
  ],
  imports: [
    BrowserModule,
    NgxStickyfillModule,
  ],
  bootstrap: [AppComponent]
})
export class AppModule {}
```

# Usage
```
<div ngxStickyfill class="top-offset">
  <h3>Hi, I'm very sticky!</h3>
</div>
```

The directive only adds the position:sticky support. To adjust the top offset, set your own css rules:

```
.top-offset{
  top:30px;
}
```