using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class NPC : MonoBehaviour
{   
    Vector3 newPosition;
    public int health = 100;
    public int level = 20;
    public int speed = 5;
    // Start is called before the first frame update
    void Start()
    {
       health+=level; 
    }

    // Update is called once per frame
    void Update()
    {
      newPosition.z += speed * Time.deltaTime;
      transform.position = newPosition;
    }
}
