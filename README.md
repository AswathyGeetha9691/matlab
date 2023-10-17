# matlab
format long
%program to evaluate the x and y displacement components at the given
%point in a 4 noded element
xi= 0.1;
eta= 0.05;
% displacement component at 4 nodal points

ue = [0.001 0.0015 0.0016 0.001; 0.001 0.0011 0.0011 0.001 ];

% calculating shape functions
shp = Shapf(xi,eta);
% x and y displacement components 
u= ue*shp';

disp(u);
