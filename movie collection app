# Movie Collection App
# storage Lists
menu_prompt="\nenter 'a' to add a movie,'l' to see your movies,'f' to find a movie , or'q' to quit :"
movies=[] #list

def addmovie(): #function addmovie
  title=input(f"enter a movie title to your collection: \n")
  director=input("enter the movie director: \n")
  year=int(input("year: \n"))
    


  movies.append({'title':title,'director':director,'year':year})
  print("suucessfuly added to the movie list")
  menu()

def showmovie():
    for movie in movies:
        print_movie(movie)
        menu()


def print_movie(movie):
     print(f"title:{movie['title']}")
     print(f"director:{movie['director']}")
     print(f"year:{movie['year']}")


def findmovie():
    search=input("enter movie title youre looking for")
    for movie in movies:
     if movie ['title']==search:
        print_movie(movie)
     menu()



useroptions={
    "a":addmovie,
    "l":showmovie,
    "f":findmovie
}
#
def menu():
 selection=input(menu_prompt)
 while selection!='q':
    if selection in useroptions:
        selected_function=useroptions[selection]
        selected_function()
        break

    else:
        print("unknown command")
        selection=input(menu_prompt)


menu()
