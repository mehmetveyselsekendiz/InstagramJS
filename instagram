User = class {
    constructor(name){
        this.name= name
        this.posts= []
        this.followers= []
        this.following= []
    }

    addPost(photoID){
        this.posts.push(new Post(photoID, this))
    }

    like(post){
        post.likes.push(this)
    }

    follow(user){
        this.following.push(user)
        user.followers.push(this)
    }

}

Post= class {
    constructor(photoID, owner){
        this.photoID= photoID
        this.owner= owner
        this.likes= []
    }
}

veysel= new User("Veysel")
ferit= new User("Ferit")

veysel.addPost(1)
ferit.follow(veysel)
ferit.like(veysel.posts[0])
