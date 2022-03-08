# Routing Optimizer

The solution based on the vehicle routing problem is in this repository described in python by me in notebook format.

Article published on Medium: https://medium.com/neogrid/desmistificando-roteiriza%C3%A7%C3%B5es-com-python-5b80f940a6fb

## Type of application
  Jupyter Notebook

## Built With
- [Python 3.10](https://www.python.org/)
- [Google OR-Tools](https://developers.google.com/optimization)
- [Pandas](https://pandas.pydata.org/)
- [Scikit-learn](https://scikit-learn.org/stable/)
- [Plotly](https://plotly.com/)
- [Mapbox](https://www.mapbox.com/)

## Getting Started

1 - For you to run the notebook, you need to have [Jupyter](https://jupyter.org/) installed on your computer or access it in the cloud.

2 - You also need to create a [Mapbox](https://www.mapbox.com/) account to get the token so you can plot the clustered routes on the map

In the notebook put your token in the following variable

```py
mapbox_token = <Your_Token>
```

3 - You need to have installed the following packages

- [Google OR-Tools](https://developers.google.com/optimization/install)
- [Pandas](https://pandas.pydata.org/docs/getting_started/install.html)
- [Scikit-learn](https://scikit-learn.org/stable/install.html)
- [Plotly](https://plotly.com/python/getting-started/)
- [Numpy](https://numpy.org/install/)

3 - Just run It

## About the project

I used in the implementation as a reference all the US states as visiting points, the spreadsheet with the data is in the project.

Further explanations about the implementation can be found in the notebook

## What is the problem?

### Travel salesman problem

One of the most famous and well-known problems in the areas of computer science and operations research is the traveling salesman problem (TSP) which consists of: Given a set of cities and their positions, the problem is to find the shortest route for each city be visited only once and finally return to the starting point.

<img src="https://i.makeagif.com/media/4-25-2016/UZrVqj.gif" alt="TSP" width="400"/>

The problem can be solved by analyzing each round-trip route to determine the shortest. However, as the number of destinations increases, the corresponding number of round trips exceeds the capabilities of even the fastest computers. With 10 destinations, there can be over 300,000 permutations and round-trip combinations. With 15 destinations, the number of possible routes could exceed 87 billion.

### Vehicle routing problem

In the Vehicle Routing Problem (VRP), the objective is to find optimal routes for multiple vehicles visiting a set of locations. (When there is only one vehicle, it boils down to the Traveling Salesman Problem.)

<img src="https://developers.google.com/optimization/images/routing/vrpgs_solution.svg" alt="VRP" width="400"/>

Vehicle routing problems are inherently intractable: the time required to resolve them grows exponentially with the size of the problem.

But what do we mean by "optimal routes" for a VRP? One answer is the routes with the shortest total distance. However, if there are no other restrictions, the ideal solution is to assign only one vehicle to visit all locations and find the shortest route for that vehicle. This is essentially the same problem as TSP.

A better way to define optimal routes is to minimize the length of the longest single route among all vehicles. This is the right definition if the goal is to complete all deliveries as quickly as possible. 


## References

[Travelling salesman problem](https://en.wikipedia.org/wiki/Travelling_salesman_problem)

[Vehicle routing problem](https://en.wikipedia.org/wiki/Vehicle_routing_problem)

[Google OR-Tools](https://developers.google.com/optimization)
 



