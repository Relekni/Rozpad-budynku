# Rozpad-budynku
Projekt koncepcyjny budynku wraz z systemem niszczenia

## Założenia
Projekt został wykonany na bazie poniższych prac koncepcyjnych, a także researchu starodawnych budynków.

![leicester_sq_1 1](https://user-images.githubusercontent.com/86862615/124340593-91b4ad00-dbb6-11eb-9de2-4abb59c32958.jpg)
![Przechwytywanie](https://user-images.githubusercontent.com/86862615/124340594-924d4380-dbb6-11eb-8311-6fce95f61b59.JPG)

Czas wykonania projektu: 7 dni
Zastosowane programy: Blender

## Model
Model został wykonany całkowicie w Blenderze z zastosowaniem technik hard surface. 
Model początkowo składał się z dużej ilości małych obiektów, a końcowo utworzony został jeden mesh przy użyciu funkcji boolean union. 
![blender_render](https://user-images.githubusercontent.com/86862615/124340664-20292e80-dbb7-11eb-9ddf-c8abecd41a06.JPG)

Siatka projektu została sprawdzona pod względem powierzchni non-manifold, składa się głównie z quadów, jednak występują także trójkąty.
![blender_original](https://user-images.githubusercontent.com/86862615/124340660-169fc680-dbb7-11eb-8f5b-8e33e3d8ee74.JPG)
![blender_original_2](https://user-images.githubusercontent.com/86862615/124340661-17d0f380-dbb7-11eb-8a48-e222b3279090.JPG)

W celu prawidłowego użytkowania modelu, należało wykonać triangulate, by umożliwić prawidłowy odczyt modelu innym programom.
![blender_triangulate](https://user-images.githubusercontent.com/86862615/124340685-4bac1900-dbb7-11eb-9fd9-e0822053f6b0.JPG)

## Zniszczenia
Zniszczenia zostały wykonane poprzez funkcję Blendera "Cell fracture".
Zaproponowane są dwa rozwiązania:
1. Użycie Cell Fracture na całym modelu w celu rozbicia go na losowe elementy:
![blender_cell_fracture](https://user-images.githubusercontent.com/86862615/124340727-82822f00-dbb7-11eb-9c79-3e27f7571cf4.JPG)

2. Podzielenie modelu na około 4 części, by uzyskać "moduły", które mogą być później niszczone oddzielnie za pomocą Cell Fracture.
![blender_moduly3](https://user-images.githubusercontent.com/86862615/124340747-a9406580-dbb7-11eb-9306-0a7e0f120337.JPG)
![blender_moduly](https://user-images.githubusercontent.com/86862615/124340745-a80f3880-dbb7-11eb-9531-1d5758c8e648.JPG)
![blender_moduly2](https://user-images.githubusercontent.com/86862615/124340746-a8a7cf00-dbb7-11eb-9fd5-afd88a3e9c3d.JPG)

## Remesh
Model po przemianie polygonów w trójkąty może zostać wykorzystany do stworzenia wersji High Poly, w celu dodania detali. Poniżej przykład siatki wygenerowanej w Zbrush.
![zbrush](https://user-images.githubusercontent.com/86862615/124340765-cb39e800-dbb7-11eb-9d34-f9c8ef4ae227.JPG)
![zbrush_2](https://user-images.githubusercontent.com/86862615/124340766-cbd27e80-dbb7-11eb-9977-48a6bdf89270.JPG)

## Teksturowanie
Model został dostosowany pod UDIM - siatka UV rozbita jest na 4 osobne tekstury, które mogą zostać stworzone np. w Substance Painterze i innych programach obsługujących UDIM.
![UDIM](https://user-images.githubusercontent.com/86862615/124340788-fcb2b380-dbb7-11eb-8963-407cbe0dad2a.JPG)
![UDIM_painter](https://user-images.githubusercontent.com/86862615/124341002-9fb7fd00-dbb9-11eb-84e5-ab5412bf8089.JPG)



