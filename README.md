Download Link: https://assignmentchef.com/product/solved-ecs175-project5-a-simple-ray-tracer
<br>
The fifth project requires the implementation of the <strong>ray tracing </strong>algorithm discussed in class. Write a program to render a scene in 3D space containing planes and other implicitly defined surfaces of degree 2 (<em>e.g.</em>, spheres and ellipsoids), and triangulated surfaces. The <strong>input parameters </strong>for the program are the <strong>from point</strong>, the <strong>at point</strong>, the <strong>up vector</strong>, and the <strong>viewing angle </strong><em>α. </em>The <strong>position of the light source(s) </strong>and the <strong>resolution </strong>of the final image (<em>N </em>× <em>N </em>pixels) will be specified by the user as well.

You must implement the <em>generalized </em>Phong illumination model considering direct and global illumination effects, given by the formula

<em>I </em>= <em>I</em><sub>direct </sub>+ <em>I</em>global

<em>,</em>

where the Phong illumination formula now incorporates the <strong>global illumination </strong>term <em>I</em><sub>global</sub><em>. </em>The values <em>I<sub>r </sub></em>and <em>I<sub>t </sub></em>are vector-valued (red, green, and blue components). They are obtained by applying the Phong illumination model recursively. All <strong>parameters in this equation are input </strong>for the ray tracer. The user can specify the color properties of each object in the scene. The global illumination term must be <strong>computed recursively </strong>as discussed in class. When computing the color/intensity for a particular pixel, stop the recursion when a user-specified <strong>maximum number of recursion levels </strong>is reached or when a reflected/refracted <strong>ray hits one of the faces of the bounding box </strong>surrounding the given scene.

For this project, you need to consider <strong>intersections </strong>between rays (=lines defined in parametric form) and implicit surfaces and between rays and triangles approximating surfaces. Use the intersection algorithms discussed in class. In order to allow <strong>transparent objects</strong>, you also need to implement the procedure for computing refracted rays. This requires the specification of <strong>refraction coefficients </strong><em>η </em>for all objects/media in the scene. The user must be able to change these. <strong>Shadow feelers </strong>must be used at each point encountered in the scene to determine whether it receives direct light from a light source or not. To satisfy the expectations for this project, when a point lies “in shadow” you do not need to consider the concept of <strong>direct transmission </strong>of light from a light source through a transparent medium that exists between the point and the light source.

The scene you render must contain <strong>at least five different surfaces </strong>(<em>e.g.</em>, plane, sphere, ellipsoid).

1

Besides having to hand in a program listing, please prepare a “manual sheet” explaining how to use your program.