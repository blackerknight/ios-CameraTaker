# ios-CameraTaker
Example take photo camera

usage:

## 1.- build variable

```
fileprivate var photoTaker: TakePhotoCamera!
```

```
override func viewDidLoad() {
super.viewDidLoad()
  photoTaker = TakePhotoCamera(vc: self)
}
```
## 2.- call for get results:

```
photoTaker.takePhoto { [weak self] (image) in
  self?.imageViewPhoto.image = image
}
```
