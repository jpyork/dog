using System;

namespace DogChallenge {
    public enum Gender {
        male,
        female,
    }

    class Dog {
        public string name;
        public string owner;
        public int age;
        public Gender gender;

        public Dog(string name, string owner, int age, Gender gender) {
            this.name = name;
            this.owner = owner;
            this.age = age;
            this.gender = gender;
        }

        public void Bark(int num) {
            for (int i = 0; i < num; i++) {
                Console.WriteLine("Woof! ");
            }
        }

        public string GetTag() {
            bool isMale = gender == Gender.male;
            return "If Lost, call " + owner + ". " + (isMale ? "His" : "Her") + " name is " + name + " and " + (isMale ? "he" : "she") + " is " + age + " year" + (age > 1 ? "s" : "") + " old.";
        }
    }
    class Program {
        static void Main() {
            Dog puppy = new Dog("Orion", "Shawn", 1, Gender.male);
            puppy.Bark(3);
            Console.WriteLine(puppy.GetTag());

            Dog myDog = new Dog("Lileu", "Dale", 4, Gender.female);
            myDog.Bark(1);
            Console.WriteLine(myDog.GetTag());
        }
    }
}
