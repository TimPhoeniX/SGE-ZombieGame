
set(GAME_SOURCE_FILES main.cpp
		Actions.cpp 
		Actions.hpp 
		Logics.cpp 
		Logics.hpp 
		Objects.cpp
		Objects.hpp
		ZombieScene.cpp
		ZombieScene.hpp
		IntroScene.cpp
		IntroScene.hpp)

add_executable(${PROJECT_NAME} ${GAME_SOURCE_FILES})

target_link_libraries(${PROJECT_NAME}
	${SGE_LIBRARIES}
	${Boost_LIBRARIES}
	${SDL2_LIBRARY}
	${GLEW_LIBRARIES}
	${OPENGL_LIBRARIES}
	${GLM_LIBRARIES}
)
