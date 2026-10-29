# Orcinus Station

Final group project for DIGI142: 3D Design for Production II, built in Unreal Engine 5.7 by Team Catilaners. This repo holds my (Erica Liang) part of the project: the train station, the Blueprints, the snow and slip systems, the VFX, and the lobby.

## Trailer

[Watch the showcase video on Vimeo](https://vimeo.com/1240581425)

## My contributions

- Helped put everything into one scene.
- Helped with final art adjustment of the scene: post processing, toning materials to keep the environment consistent, lighting and fog.

### Train station

- Modelled and textured the train station.
- `BP_Pendulum` and `BP_MiniPendulum` for the pendulums.

### Global MPC snow control

- A material function (`MF_Snow`) and a material parameter collection (`MPC_Snow`) that globally control and blend snow onto any other material in the scene.
- The snow material itself is from FAB.

### Slipping snow

- A physical material that can be attached to materials to make a surface slippery.

### Car, train and gear spawners

- `BP_CarSpawner`, `BP_TrainSpawner` and `BP_GearSpawner`.
- Cars get a random colour variation when they spawn.

### Train smoke Niagara collision

- Smoke particles that collide with the scene. The smoke material is from FAB.

### Water spark Niagara system

- Sparks on the water that tell the player the water is dangerous (`M_Spark` graph).

### Lobby screen, logo and banner pictures

- Lobby screen, title logo, and banner pictures for everyone on the team (except Alley).
- Character selection works in the lobby, but the group never got the lobby to game character transition working. The selection does not carry over to the character index in game, so the playable character is randomised in game for now.

Screenshots, wireframes and Blueprint graphs are in the write-up: [`docs/EricaLiang_Assignment03_GroupProject.pdf`](docs/EricaLiang_Assignment03_GroupProject.pdf).

## What is in this repo

This is a trimmed copy of the project, not a full open-and-play project. The full project is about 25 GB and includes third-party marketplace packs that cannot be redistributed, so these are left out:

- Third-party environment packs and their maps.
- Large baked maps and `*_BuiltData` files.
- Snow and smoke textures and other FAB assets.

Included: `Config/`, the `.uproject`, the Blueprints (`Content/_STUDENT_CONTENT/Project_Assets/Blueprints`), my own folder (`Erica/`), and the base materials and material instances.

## Team

Team Catilaners. This repo only covers my own contributions.

## Credits

Snow and smoke materials are from FAB, used under their own licences. Other third-party assets are credited in the project write-up.
