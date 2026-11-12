## Imagine Online education platform:

Every student has a name and ID.A student can be either a Regular Student or a Premium Student.Regular students have enrolled courses.
Premium students have enrolled courses and additional benefits.




//type Student = {
  id: number;
  name: string;
  email: string;
};

type RegularStudent = {
  role: "regular";
  enrolledCourses: string[];
};

type PremiumStudent = {
  role: "premium";
  enrolledCourses: string[];
  benefits: string[];
};

// Intersection (&)
type Regular = Student & RegularStudent;
type Premium = Student & PremiumStudent;

// Union (|)
type StudentAccount = Regular | Premium;