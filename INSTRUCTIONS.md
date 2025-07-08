# Instructions to test the repository

1.  **Add Haskell to your PATH:** Before you can build or run any Haskell code, you need to add the Haskell binaries to your system's PATH. This will allow you to run `ghc` and `cabal` from the command line.
2.  **Build the project:** Open a terminal in the root of the repository and run the following command: `cabal build`. This command will download any necessary dependencies and compile the project, creating an executable file.
3.  **Run the executable:** Once the project is built, you can run the executable with the following command: `cabal run cpr -- unrank <integer>`. Replace `<integer>` with the integer you want to convert to a chess position.
4.  **Verify the output:** The command will output a chess position in FEN format. To verify that the conversion is correct, you can then run `cabal run cpr -- rank <fen>` to convert the FEN string back to the original integer.