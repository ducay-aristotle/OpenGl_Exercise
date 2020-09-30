## OpenGl_Exercise
This project was created mainly because of my slight interest with c++ and working glfw to make interactive games.

## Project Description(Detailed)
The reason for working on this project is to have a personal in progress project so that I may have a baseline for working with OpenGL and C++. 

## Source Code
    Window Source Code:
    int main()
    {
	//initialize GLFW
	glfwInit();

	//CREATE WINDOW
	const int WINDOW_WIDTH = 640;
	const int WINDOW_HEIGHT = 48; //WINDOW AND FRAME BUFFERS SHOULD BE SAME SIZE
	int framebufferWidth = 0;
	int framebufferHeight = 0;			
	//USING CORE PROFILE
	glfwWindowHint(GLFW_OPENGL_PROFILE, GLFW_OPENGL_CORE_PROFILE);
	//4.4(MAJOR 4 . MINOR 4)
	glfwWindowHint(GLFW_CONTEXT_VERSION_MAJOR, 3);
	glfwWindowHint(GLFW_CONTEXT_VERSION_MINOR, 3);
	//Window Resize property
	glfwWindowHint(GLFW_RESIZABLE,GL_FALSE);

	//Width, Height, Title of window, borderless/fullscreen mode,
	//can share window
	GLFWwindow* window = glfwCreateWindow(WINDOW_WIDTH, WINDOW_HEIGHT, "OpenGLWindowExercise", NULL, NULL);
	glfwGetFramebufferSize(window, &framebufferWidth, &framebufferHeight);
	glViewport(0, 0, framebufferWidth, framebufferHeight);
	glfwMakeContextCurrent(window); //IMPORTANT

	//INIT GLEW (NEEDS WINDOW AND OPENGL CONTEXT)
	glewExperimental = GL_TRUE;

## Skills Aquired/Learned
- Function fundamentals when working with C++
- making/linking dynamic libraries to a project file
- Experience working with OpenGL
- Workflow when working with C++ and OpenGL
