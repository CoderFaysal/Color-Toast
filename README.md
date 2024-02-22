# Color Toast

## Prerequisites
Add this in your root settings.gradle.kts (Project Settings) :

```
dependencyResolutionManagement {
    repositories {

        maven { url = uri("https://www.jitpack.io" ) }

    }
}
```

## Dependency
Add this to your module's build.gradle.kts (Module : app)

```
dependencies {

    implementation("com.github.GrenderG:Toasty:1.5.2")

}
```

## Usage

To display an error Toast:
```
Toasty.error(yourContext, "This is an error toast.", Toast.LENGTH_SHORT, true).show();
```

To display a success Toast:
```
Toasty.success(yourContext, "Success!", Toast.LENGTH_SHORT, true).show();
```

To display an info Toast:
```
Toasty.info(yourContext, "Here is some info for you.", Toast.LENGTH_SHORT, true).show();
```

To display a warning Toast:
```
Toasty.warning(yourContext, "Beware of the dog.", Toast.LENGTH_SHORT, true).show();
```

To display the usual Toast:
```
Toasty.normal(yourContext, "Normal toast w/o icon").show();
```

To display the usual Toast with icon:
```
Toasty.normal(yourContext, "Normal toast w/ icon", yourIconDrawable).show();
```

You can also create your custom Toasts with the custom() method:
```
Toasty.custom(yourContext, "I'm a custom Toast", yourIconDrawable, tintColor, duration, withIcon, 
shouldTint).show();
```


## Screenshots
<img src="https://raw.githubusercontent.com/GrenderG/Toasty/master/art/collage.png"/>

