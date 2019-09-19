# Build your library and schematics

From the root of your workspace, run the `ng build` command for your library.


> `ng build my-lib`

Then, you change into your library directory to build the schematic


> ```cd projects/my-lib```

> ```npm run build```

## Link the library
Your library and schematics are packaged and placed in the dist/my-lib folder at the root of your workspace. For running the schematic, you need to link the library into your **node_modules** folder. From the root of your workspace, run the `npm link` command with the path to your distributable library.


> `npm link dist/my-lib`

## Run the schematic

Now that your library is installed, you can run the schematic using the ng generate command.


> ```ng generate my-lib:my-service --name my-data```

In the console, you will see that the schematic was run and the `my-data.service.ts` file was created in your app folder.

> CREATE src/app/my-data.service.ts (208 bytes)