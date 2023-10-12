# to start toplevel from command prompt
eval `opam config env`
utop
 
# Compile
ocamlc -o hello.byte hello.ml
# execute 
./hello.byte

# clean up
rm -rf hello.byte hello.cmi hello.cmo


# building using dune
Create a dune file and put

(executable
 (name hello))
 

 Create a dune-proj and put 
 (lang dune 3.4)


 dune build hello.exe

 dune exec ./hello.exe

 dune clean