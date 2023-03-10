
# DEVS Notesπ

Note-taking app local database "Sqflite"\
With all its own operationsπ:\
CRUD system.

![](https://user-images.githubusercontent.com/60518534/211018545-a1ee81f8-7b2c-492e-ade8-e1a588df34cd.gif)
#### [Video](https://www.linkedin.com/posts/mahmoudalaa2210_bloc-flutterabrbloc-sqflite-activity-7005512754648264705-AdpS?utm_source=share&utm_medium=member_desktop)

## Download App 
<a href="https://github.com/MahmoudAlaa22/DEVS-Notes-Readme-file/releases/download/V1.0/app-release.apk"><img src="https://playerzon.com/asset/download.png" width="200"></img></a>
## β Tools Used
- Flutter 
- Dart
- Database (Sqflite)
- lottie


## β¨ Features
β Light & Dark mode.\
β You can write βοΈ.\
β Record π\
β Put a picture πΈ.\
β Draw π¨ the note you want πβ€οΈ.\
β You can change the color of the note with the color you want π€©.\
β The app also supports Arabic and English π\
β The design is suitable for all screen sizesπβ¨


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
β
βββββ core
β     ββββ app_prefs
β     β    βββ app_prefs.dart
β     ββββ assets
β     β    βββ images
β     β         βββ app_images.dart
β     ββββ config
β     β    βββ responsive_app.dart
β     ββββ constant
β     β     βββ strings.dart
β     ββββ controller
β     β     βββ audio_bloc
β     β         βββ cubit
β     β             βββ audio_cubit.dart
β     β             βββ audio_state.dart
β     ββββ error
β     β     βββ exceptions.dart
β     β     βββ failures.dart
β     ββββ language
β     β     βββ language_manager.dart
β     ββββ routes
β     β     βββ router.dart
β     β     βββ routes.dart
β     ββββ service
β     β     βββ file_service.dart
β     β     βββ image_picker_service.dart
β     β     βββ vibration_service.dart
β     ββββ sql
β     β     βββ init_database.dart
β     β     βββ sql_constants.dart
β     ββββ theme
β     β     βββ bloc
β     β     β   βββ cubit
β     β     β       βββ theme_cubit.dart
β     β     β       βββ theme_state.dart
β     β     βββ colors.dart
β     β     βββ themes.dart
β     ββββ validators
β     β     βββ validate_messages.dart
β     β     βββ validators.dart
β     ββββ bloc_observer.dart
β
βββββ features
β     ββββ note
β     β     βββ data
β     β     β   ββββ datasources
β     β     β   β   βββ note_local_datasources.dart
β     β     β   ββββ model
β     β     β   β   βββ note_model.dart
β     β     β   ββββ repositories
β     β     β       βββ note_repo_impl.dart
β     β     βββ domain
β     β     β   ββββ repositories
β     β     β   β   βββ note_repo.dart
β     β     β   ββββ usecases
β     β     β       ββββ add_note_usecase.dart
β     β     β       ββββ delete_note_usecase.dart
β     β     β       ββββ get_notes_usecase.dart
β     β     β       ββββ update_note.dart
β     β     βββ presentation
β     β         ββββ bloc
β     β         β   βββ cubit
β     β         β       βββ add_note
β     β         β       β   βββ add_note_cubit.dart
β     β         β       β   βββ add_note_state.dart
β     β         β       βββ get_notes
β     β         β           βββ get_notes_cubit.dart
β     β         β           βββ get_notes_state.dart
β     β         ββββ pages
β     β              βββ add_note
β     β              β   βββ widgets
β     β              β   β   βββ add_note_form.dart
β     β              β   β   βββ bottom_sheet_add_note.dart
β     β              β   β   βββ record_widget.dart
β     β              β   β   βββ slider_widget.dart
β     β              β   β   βββ text_form_add_note.dart
β     β              β   βββ add_note_page.dart
β     β              βββ notes
β     β              β   βββ widgets
β     β              β   β   βββ add_note_button.dart
β     β              β   β   βββ app_bar_widget.dart
β     β              β   β   βββ bottom_sheet_widget.dart
β     β              β   β   βββ custom_painter.dart
β     β              β   β   βββ empty_notes.dart
β     β              β   β   βββ icon_button_image.dart
β     β              β   β   βββ icon_button_mic.dart
β     β              β   β   βββ note_item.dart
β     β              β   β   βββ show_dialog_audio_recording.dart
β     β              β   βββ notes_page.dart
β     β              βββ search_notes
β     β              β   βββ widgets
β     β              β   β   βββ empty_search_note.dart
β     β              β   β   βββ search_appbar.dart
β     β              β   βββ search_notes.dart
β     β              βββ home_page.dart
β     β
β     ββββ drawing_page ...
β     ββββ splash ...
β
βββββ widgets
β     ββββ action_button.dart
β     ββββ animated_button_widget.dart
β     ββββ drawer_page.dart
β     ββββ flutter_toast_widget.dart
β     ββββ grid_view_notes.dart
β     ββββ list_tile_item_widget.dart
β     ββββ flutter_toast_widget.dart
β     ββββ list_tile_item_widget.dart
β     ββββ loader_widget.dart
β     ββββ mode_theme_widget.dart
β     ββββ text_widget.dart
β
βββββ injection_container.dart
βββββ main.dart    
```


## Packages

![image](https://user-images.githubusercontent.com/60518534/211029565-8b2d2f5e-deaa-4bb8-87b1-8a4fca30cc9b.png)
## Feedback

If you have any feedback, please reach out to us at mahmoud3laa2210@gmail.com

## π You can follow me on

[![portfolio](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/MahmoudAlaa22)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mahmoudalaa2210/)
