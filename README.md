# proyecto-final-de-poo

Proyecto final de Programación Orientada a Objetos (POO).

Proyecto Java 17 con Maven. Cada quien puede usar el editor que quiera
(IntelliJ IDEA, VS Code, Eclipse, NetBeans): todos abren el `pom.xml` igual,
y los archivos propios de cada editor están en el `.gitignore`, así que no se cuelan al repo.

## Estructura

```
src/main/java/poo/   <- código del proyecto (Main.java es el punto de entrada)
src/test/java/poo/   <- pruebas (JUnit 5)
pom.xml              <- configuración del proyecto
```

## Primera vez (cada integrante)

1. Acepta la invitación de colaborador que te llega por correo/GitHub.
2. Instala Git y un JDK 17 o más nuevo.
3. Configura tu nombre (solo una vez por compu):
   ```
   git config --global user.name "Tu Nombre"
   git config --global user.email "tu-correo-de-github@ejemplo.com"
   ```
4. Clona el repo:
   ```
   git clone https://github.com/adangarciaj/proyecto-final-de-poo.git
   ```
5. Ábrelo en tu editor:
   - **IntelliJ:** File → Open → elige la carpeta (detecta el `pom.xml` solo).
   - **VS Code:** abre la carpeta y acepta instalar las extensiones recomendadas (Extension Pack for Java).
   - **Eclipse:** File → Import → Existing Maven Projects.
   - **NetBeans:** File → Open Project.
6. Corre `poo.Main` para comprobar que todo jala.

## Flujo de trabajo

Antes de empezar a trabajar, **siempre** baja lo último:

```
git pull
```

Cuando termines algo:

```
git add .
git commit -m "Agrega clase Cliente con sus getters"
git pull
git push
```

Recomendado si van a trabajar varios a la vez: cada quien en su rama y luego Pull Request.

```
git checkout -b nombre-o-tarea
# ... trabajas y haces commits ...
git push -u origin nombre-o-tarea
```

Después en GitHub: **Compare & pull request** → otro integrante lo revisa → **Merge**.

## Reglas para no pelearnos con Git

- Hagan `git pull` antes de empezar y antes de hacer `push`.
- Commits chicos y con mensaje que diga qué hiciste.
- No suban carpetas `target/`, `out/`, `.idea/`: ya están ignoradas.
- Si dos tocan el mismo archivo y sale conflicto, abran el archivo, quédense con lo correcto,
  borren las marcas `<<<<<<<`, `=======`, `>>>>>>>` y hagan commit.
