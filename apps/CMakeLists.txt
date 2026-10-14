#add the executable target named HelloWorld
add_executable(greet greet.cpp)
target_link_libraries(greet PRIVATE greeter)

# Executable greet, built from greet.cpp and using the library greeter
install(TARGETS greet 
    DESTINATION bin
)
