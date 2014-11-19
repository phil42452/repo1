repo1
=====

Simple class that provides easy gravatar integration

#Getting the avatar

First you need to create a oGravatar object, see below:
    
    $my_gravatar = new oGravatar('phil42452@gmail.com');

If you want to use a secure connection, you'll need to pass `true` as second parameter.

Now that you have the object created, you can set the some properties like the image size, rating and a default image, in case of a non Gravatar account.

##Image Size

Simply use the `setSize` function and use an integer greater than 1 and less than 2048 for the pixel size.

    $my_gravatar->setSize(200);

##Image Rating

The function you need is `setRating` and you can use one of the following constants to simplify your life:

- `oGravatar::RATING_G`
- `oGravatar::RATING_PG`
- `oGravatar::RATING_R`
- `oGravatar::RATING_X`

Just like this:

    $my_gravatar->setRating(oGravatar::RATING_X);
    
##Default Image
