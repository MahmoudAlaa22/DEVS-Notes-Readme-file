
# DEVS Notes📚

Note-taking app local database "Sqflite"
With all its own operations👌:
CRUD system.

![E-Commerce App (1)](https://user-images.githubusercontent.com/60518534/211018545-a1ee81f8-7b2c-492e-ade8-e1a588df34cd.gif)
#### [Video](https://www.linkedin.com/posts/mahmoudalaa2210_bloc-flutterabrbloc-sqflite-activity-7005512754648264705-AdpS?utm_source=share&utm_medium=member_desktop)

## Download App 
<a href="[https://github.com/MahmoudAlaa22/DEVS-Notes-Readme-file/releases/download/V1.0/app-release.apk](https://github.com/MahmoudAlaa22/E-Commerce-Readme-file-/releases/download/V1.0/app-release.apk)"><img src="https://playerzon.com/asset/download.png" width="200"></img></a>

## ⚙ Tools Used
- Flutter 
- Dart
- Database (Sqflite)
- lottie


## ✨ Features
✔ Light & Dark mode.\
✔ You can write ✍️.\
✔ Record 🎙\
✔ Put a picture 📸.\
✔ Draw 🎨 the note you want 👌❤️.\
✔ You can change the color of the note with the color you want 🤩.\
✔ The app also supports Arabic and English 🌐\
✔ The design is suitable for all screen sizes👌✨


# Screenshots
## Light Mode

  Splash Page                 |   Home Page        |  Drawer Page
:-------------------------:|:-------------------------:|:-------------------------:
![](https://user-images.githubusercontent.com/60518534/211012094-4d8fc763-d4d2-4184-92ac-402f3a723da4.jpg)|![](https://user-images.githubusercontent.com/60518534/211012100-7b62e186-f14d-468d-8d4d-ad7a4b275ce7.jpg)|![](https://user-images.githubusercontent.com/60518534/211012122-cb194488-0bdc-42a3-87ef-40aae0a80fa0.jpg)

  Add Note Page                 |   Drawing Page        |  Searching Page
:-------------------------:|:-------------------------:|:-------------------------:
![](https://user-images.githubusercontent.com/60518534/211012131-e207b4cc-703b-4302-8eee-2629d4db5f01.jpg)|![](https://user-images.githubusercontent.com/60518534/211024575-b8e0745f-c2aa-47f3-8589-8f825377b352.jpg)|![](https://user-images.githubusercontent.com/60518534/211012156-ac1b53d4-56c6-40b0-b02e-0b80fe26f48c.jpg)

## Dark Mode

  Splash Page                 |   Home Page        |  Drawer Page
:-------------------------:|:-------------------------:|:-------------------------:
![](https://user-images.githubusercontent.com/60518534/211012182-78ec4085-96a8-488e-b2b4-03fd28f15728.jpg)|![](https://user-images.githubusercontent.com/60518534/211012031-e7d55546-1e05-4f5b-acf8-019b918273f8.jpg)|![](https://user-images.githubusercontent.com/60518534/211012052-15ae35f7-4d56-4b20-8622-5e890afc0ffb.jpg)

  Add Note Page                 |   Drawing Page        |  Searching Page
:-------------------------:|:-------------------------:|:-------------------------:
![](https://user-images.githubusercontent.com/60518534/211012058-ec7f7138-9e3f-4849-aca1-ccc2d17a5653.jpg)|![](https://user-images.githubusercontent.com/60518534/211024590-fd038650-0f31-4e5d-9a1f-36e702dec134.jpg)|![](https://user-images.githubusercontent.com/60518534/211012076-a3663560-495a-420c-841d-f8709ee12234.jpg)



## Directory Structure

```
lib
│
│──── core
│     │─── app_prefs
│     │    └── app_prefs.dart
│     │─── assets
│     │    └── images
│     │         └── app_images.dart
│     │─── config
│     │    └── responsive_app.dart
│     │─── constant
│     │     └── strings.dart
│     │─── controller
│     │     └── audio_bloc
│     │         └── cubit
│     │             │── audio_cubit.dart
│     │             └── audio_state.dart
│     │─── error
│     │     │── exceptions.dart
│     │     └── failures.dart
│     │─── language
│     │     └── language_manager.dart
│     │─── routes
│     │     │── router.dart
│     │     └── routes.dart
│     │─── service
│     │     │── file_service.dart
│     │     │── image_picker_service.dart
│     │     └── vibration_service.dart
│     │─── sql
│     │     │── init_database.dart
│     │     └── sql_constants.dart
│     │─── theme
│     │     │── bloc
│     │     │   └── cubit
│     │     │       │── theme_cubit.dart
│     │     │       └── theme_state.dart
│     │     │── colors.dart
│     │     └── themes.dart
│     │─── validators
│     │     │── validate_messages.dart
│     │     └── validators.dart
│     └─── bloc_observer.dart
│
│──── features
│     │─── note
│     │     │── data
│     │     │   │─── datasources
│     │     │   │   └── note_local_datasources.dart
│     │     │   │─── model
│     │     │   │   └── note_model.dart
│     │     │   └─── repositories
│     │     │       └── note_repo_impl.dart
│     │     │── domain
│     │     │   │─── repositories
│     │     │   │   └── note_repo.dart
│     │     │   └─── usecases
│     │     │       │─── add_note_usecase.dart
│     │     │       │─── delete_note_usecase.dart
│     │     │       │─── get_notes_usecase.dart
│     │     │       └─── update_note.dart
│     │     └── presentation
│     │         │─── bloc
│     │         │   └── cubit
│     │         │       │── add_note
│     │         │       │   │── add_note_cubit.dart
│     │         │       │   └── add_note_state.dart
│     │         │       └── get_notes
│     │         │           │── get_notes_cubit.dart
│     │         │           └── get_notes_state.dart
│     │         └─── pages
│     │              │── add_note
│     │              │   │── widgets
│     │              │   │   │── add_note_form.dart
│     │              │   │   │── bottom_sheet_add_note.dart
│     │              │   │   │── record_widget.dart
│     │              │   │   │── slider_widget.dart
│     │              │   │   └── text_form_add_note.dart
│     │              │   └── add_note_page.dart
│     │              │── notes
│     │              │   │── widgets
│     │              │   │   │── add_note_button.dart
│     │              │   │   │── app_bar_widget.dart
│     │              │   │   │── bottom_sheet_widget.dart
│     │              │   │   │── custom_painter.dart
│     │              │   │   │── empty_notes.dart
│     │              │   │   │── icon_button_image.dart
│     │              │   │   │── icon_button_mic.dart
│     │              │   │   │── note_item.dart
│     │              │   │   └── show_dialog_audio_recording.dart
│     │              │   └── notes_page.dart
│     │              │── search_notes
│     │              │   │── widgets
│     │              │   │   │── empty_search_note.dart
│     │              │   │   └── search_appbar.dart
│     │              │   └── search_notes.dart
│     │              └── home_page.dart
│     │
│     │─── drawing_page ...
│     └─── splash ...
│
│──── widgets
│     │─── action_button.dart
│     │─── animated_button_widget.dart
│     │─── drawer_page.dart
│     │─── flutter_toast_widget.dart
│     │─── grid_view_notes.dart
│     │─── list_tile_item_widget.dart
│     │─── flutter_toast_widget.dart
│     │─── list_tile_item_widget.dart
│     │─── loader_widget.dart
│     │─── mode_theme_widget.dart
│     └─── text_widget.dart
│
│──── injection_container.dart
└──── main.dart    
```


## Packages

![image](https://user-images.githubusercontent.com/60518534/211029565-8b2d2f5e-deaa-4bb8-87b1-8a4fca30cc9b.png)
## Feedback

If you have any feedback, please reach out to us at mahmoud3laa2210@gmail.com

## 🔗 You can follow me on

[![portfolio](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/MahmoudAlaa22)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mahmoudalaa2210/)
