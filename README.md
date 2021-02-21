# WebApplication for Event Registration

## AIM:
To create a UX design and develop a web application for event registration.
## DESIGN STEPS:
### Step 1: 
Requirement collection.
### Step 2:
Choosing the suitable color scheme
### Step 3:
Creating artboards for individual pages
### Step 4:
Designing layout for individual pages
### Step 5:
Creating links and linking it with artboards
### Step 6:
Preview the prototype.

## DESIGN SCREENS:
![output](./static/img/d1.jpg)

![output](./static/img/d2.jpg)

![output](./static/img/d3.jpg)

![output](./static/img/d4.jpg)

![output](./static/img/d5.jpg)

## WIREFRAME:
![output](./static/img/wireframe.jpg)

## PROTOTYPE:
![output](./static/img/prototype.jpg)

## PROGRAM:
### home.html
```
<!doctype html>
<html lang="en">

<head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css"
        integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">

    <title>Saveetha Engineering College</title>
</head>

<body>
    <div class="jumbotron">
        <div class="container">
        <h1 class="display-4 text-center">Algorythm</h1>
        <p class="lead text-center">Tune yourself to our bit.</p>
        <hr class="my-4">
        <p class="text-center">Department of Artificial Intelligence and Data Science</p>
        <p class="lead text-center">
            <a class="btn btn-primary btn-lg" href="#" role="button">Learn More</a>
        </p>
        </div>
    </div>
    <div class="container">
        <div class="row">
            <div class="col-12 text-center">
                <h1>Join us and have fun.</h1>
                <div class="col-12 text-center">
                    <a href="/register" class="btn btn-primary btn-lg" role="button" aria-disabled="true">Register</a>
                </div> 
            </div>
        </div>
    </div>

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.2.1.slim.min.js"
        integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN"
        crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js"
        integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q"
        crossorigin="anonymous"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js"
        integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl"
        crossorigin="anonymous"></script>
</body>

</html>
```

### register.html
```
<!doctype html>
<html lang="en">

<head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css"
        integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">

    <title>Saveetha Engineering College</title>
</head>

<body>
    <div class="jumbotron">
        <div class="container">
            <h1 class="display-4 text-center">Algorythm</h1>
            <p class="lead text-center">Tune yourself to our bit.</p>
            <hr class="my-4">
            <p class="text-center">Department of Artificial Intelligence and Data Science</p>
            <p class="lead text-center">
                <a class="btn btn-primary btn-lg" href="#" role="button">Learn More</a>
            </p>
        </div>
    </div>
    <div class="container">
        <div class="row">
            <div class="col-12">
                <h1>Application</h1>
                <form action="/register/" method="POST">
                    {% csrf_token %}
                    <div class="form-group">
                        <label for="Name">Name</label>
                        <input type="name" class="form-control" name="Name" id="Name" placeholder="Name">
                    </div>
                    <div class="form-group">
                        <label for="Phone">Phone</label>
                        <input type="phone" class="form-control" name="Phone" id="Phone" placeholder="Phone">
                    </div>
                    <div class="form-group">
                        <label for="Email1">Email address</label>
                        <input type="email" class="form-control" name="Email1" id="Email1" aria-describedby="emailHelp"
                            placeholder="Enter email">
                        <small id="emailHelp" class="form-text text-muted">We'll never share your email with anyone
                            else.</small>
                    </div>
                    <div class="form-group">
                        <label for="Institution">Institution Name</label>
                        <input type="institution" class="form-control" name="Institution" id="Institution" placeholder="Institution Name">
                    </div>
                    <div class="form-check">
                        <input type="checkbox" class="form-check-input" name="examplecheck1" id="exampleCheck1">
                        <label class="form-check-label" for="exampleCheck1">Check me out</label>
                    </div>
                    <button type="submit" class="btn btn-primary">Procced</button>
                </form>
            </div>
        </div>
    </div>

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.2.1.slim.min.js"
        integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN"
        crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js"
        integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q"
        crossorigin="anonymous"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js"
        integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl"
        crossorigin="anonymous"></script>
</body>

</html>
```

### success.html
```
<!doctype html>
<html lang="en">

<head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css"
        integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">

    <title>Saveetha Engineering College</title>
</head>

<body>
    <div class="jumbotron">
        <div class="container">
            <h1 class="display-4 text-center">Algorythm</h1>
            <p class="lead text-center">Tune yourself to our bit.</p>
            <hr class="my-4">
            <p class="text-center">Department of Artificial Intelligence and Data Science</p>
            <p class="lead text-center">
                <a class="btn btn-primary btn-lg" href="#" role="button">Learn More</a>
            </p>
        </div>
    </div>
    <div class="container">
        <div class="row">
            <div class="col-12 text-center">
                <h1>Join us and have fun.</h1>
                <div class="col-12 text-center">
                    <a href="/home" class="btn btn-primary btn-lg" role="button" aria-disabled="true">Home</a>
                </div>
                <div class="text-center">
                    <div class="alert alert-success" role="alert">
                        <h4 class="alert-heading">Congratulations!</h4>
                        <p>Your Registration is Successful.</p>
                        <hr>
                        <h4 class="alert-heading">Thank You.</h4>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.2.1.slim.min.js"
        integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN"
        crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js"
        integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q"
        crossorigin="anonymous"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js"
        integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl"
        crossorigin="anonymous"></script>
</body>

</html>
```

### failed.html
```
<!doctype html>
<html lang="en">

<head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css"
        integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">

    <title>Saveetha Engineering College</title>
</head>

<body>
    <div class="jumbotron">
        <div class="container">
            <h1 class="display-4 text-center">Algorythm</h1>
            <p class="lead text-center">Tune yourself to our bit.</p>
            <hr class="my-4">
            <p class="text-center">Department of Artificial Intelligence and Data Science</p>
            <p class="lead text-center">
                <a class="btn btn-primary btn-lg" href="#" role="button">Learn More</a>
            </p>
        </div>
    </div>
    <div class="container">
        <div class="row">
            <div class="col-12 text-center">
                <h1>Join us and have fun.</h1>
                <div class="col-12 text-center">
                    <a href="/home" class="btn btn-primary btn-lg" role="button" aria-disabled="true">Home</a>
                </div>
                <div class="text-center">
                    <div class="alert alert-success" role="alert">
                        <h4 class="alert-heading">Sorry!</h4>
                        <p>All the seats are booked.</p>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.2.1.slim.min.js"
        integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN"
        crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js"
        integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q"
        crossorigin="anonymous"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js"
        integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl"
        crossorigin="anonymous"></script>
</body>

</html>
```

### participants.html
```
<!doctype html>
<html lang="en">

<head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css"
        integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">

    <title>Saveetha Engineering College</title>
</head>

<body>
    <div class="jumbotron">
        <div class="container">
             <h1 class="display-4 text-center">Algorythm</h1>
            <p class="lead text-center">Tune yourself to our bit.</p>
            <hr class="my-4">
            <p class="text-center">Department of Artificial Intelligence and Data Science</p>
            <p class="lead text-center">
                <a class="btn btn-primary btn-lg" href="#" role="button">Learn more</a>
            </p>
        </div>
    </div>
    <div class="container">
        <div class="row">
            <div class="col-12">
                <h1>Participants List</h1>
            </div>
        </div>
        <div class="row">
            <div class="col-12">
                <table class="table">
                    <thead>
                        <tr>
                            <th scope="col">NAME</th>
                            <th scope="col">EMAIL</th>
                            <th scope="col">PHONE</th>
                            <th scope="col">INSTITUTION</th>
                        </tr>
                    </thead>
                    <tbody>

                        <tr>
                            <td>Kavya</td>
                            <td>kavya@gmail.com</td>
                            <td>9618146729</td>
                            <td>Saveetha Engineering College</td>
                        </tr>

                        <tr>
                            <td>Sravya</td>
                            <td>Sravya@gmail.com</td>
                            <td>8074030772</td>
                            <td>Narayana Dental College</td>
                        </tr>

                        <tr>
                            <td>otto</td>
                            <td>otto@gmail.com</td>
                            <td>123</td>
                            <td>Saveetha</td>
                        </tr>

                        <tr>
                            <td>kala</td>
                            <td>kala88@gmail.com</td>
                            <td>56780</td>
                            <td>Loyola University</td>
                        </tr>

                        <tr>
                            <td>Raja</td>
                            <td>Raja22@</td>
                            <td>12380</td>
                            <td>Sasta University</td>
                        </tr>

                        <tr>
                            <td>Samu</td>
                            <td>Samu@gmail.com</td>
                            <td>14356</td>
                            <td>Sri Sai Ram University</td>
                        </tr>

                        <tr>
                            <td>Manju</td>
                            <td>Anju32@gmail.com</td>
                            <td>223345</td>
                            <td>Panimalar University</td>
                        </tr>

                        <tr>
                        <tr>
                            <td>Charitha</td>
                            <td>cherry03@gmail.com</td>
                            <td>9032460772</td>
                            <td>Geethanjali University</td>
                        </tr>

                        <tr>
                            <td>Sushma</td>
                            <td>sunny14@gmail.com</td>
                            <td>9080706050</td>
                            <td>Venkateswara University</td>
                        </tr>

                        <tr>
                            <td>Pratyushae</td>
                            <td>pratyu@gmail.com</td>
                            <td>9440567890</td>
                            <td>Rao's Engineering College</td>
                        </tr>

                        <tr>
                            <td>Khadyotha</td>
                            <td>chinni@gmail.com</td>
                            <td>9492939495</td>
                            <td>Vidyanikethan University</td>
                        </tr>

                        <tr>
                            <td>Rohith</td>
                            <td>danger@gmail.com</td>
                            <td>9989123456</td>
                            <td>Johnson University</td>
                        </tr>

                        <tr>
                            <td>Teju</td>
                            <td>teju22@gmail.com</td>
                            <td>9678745632</td>
                            <td>Veltech University</td>
                        </tr>

                        <tr>
                            <td>Mahi</td>
                            <td>Mahi27@gmail.com</td>
                            <td>9949496357</td>
                            <td>Sastra University</td>
                        </tr>

                         <tr>
                            <td>Gopi</td>
                            <td>gopi26@gmail.com</td>
                            <td>2326023</td>
                            <td>R.M.K. University</td>
                        </tr>


                    </tbody>
                </table>
            </div>
        </div>
        <div class="row">
            <div class="col-12 text-center">
                <a href="/home/" class="btn btn-primary btn-lg" role="button">Home</a>
            </div>
        </div>
    </div>

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.2.1.slim.min.js"
        integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN"
        crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js"
        integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q"
        crossorigin="anonymous"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js"
        integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl"
        crossorigin="anonymous"></script>
</body>

</html>
```

## OUTPUT:
![output](./static/img/home.jpg)

![output](./static/img/login.jpg)

![output](./static/img/participants.jpg)

![output](./static/img/success.jpg)


## RESULT:
Thus, a ux design is created and a web application is developed for event registration in the url http://kavya.student.saveetha.in:8000/home/.