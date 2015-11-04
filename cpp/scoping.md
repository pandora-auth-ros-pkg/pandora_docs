Scoping
===
----


## Namespaces

Suppose we have the following structure in a repo


- pandora_vision (meta package)
    - pandora_vision_hazmat
    - pandora_vision_obstacle (meta package)
        - pandora_vision_hard_obstacle

#### Rules

1. Every source file should be written under a namespace, **tests included**.
2. Namespaces should **not** be indented.
3. Code should start in the **same** indendation level as the namespaces.

---

**Good**:

```cpp
namespace pandora_vision {
namespace pandora_vision_obstacle {
namespace pandora_vision_hard_obstacle {

class HardObstacleDetector: public ObstacleDetector
{
  public:
    HardObstacleDetector();
    ~HardObstacleDetector();
  private:
    int findElevationMap();
};

}  // pandora_vision_hard_obstacle
}  // pandora_vision_obstacle
}  // pandora_vision
```

**Bad**

```cpp
namespace pandora_vision {
  namespace pandora_vision_obstacle {
    namespace pandora_vision_hard_obstacle {

      class HardObstacleDetector: public ObstacleDetector
      {
        public:
          HardObstacleDetector();
          ~HardObstacleDetector();
        private:
          int findElevationMap();
      };

    }  // pandora_vision_hard_obstacle
  }  // pandora_vision_obstacle
}  // pandora_vision
```
